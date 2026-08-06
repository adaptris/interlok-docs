## Overview

The `embedded-scripting-service` is a powerful and flexible component within Interlok that allows developers to execute arbitrary scripts, most commonly JavaScript via the GraalJS engine, directly within a workflow. While this flexibility is valuable during rapid prototyping or for handling highly bespoke logic, it comes with significant runtime costs that make it unsuitable as a general purpose tool in production integrations.

This guide explains the technical reasons behind those costs, demonstrates concrete migration examples from scripted implementations to native Interlok services, and provides a decision framework for when embedded scripting is and is not appropriate.

> **Production Recommendation**
>
> Treat `embedded-scripting-service` as a last resort. Always evaluate whether a native Interlok service can fulfil the same requirement before reaching for an embedded script. In high throughput or long running deployments, embedded scripts are a primary source of memory pressure and CPU spikes.

---

## Why Embedded Scripts Are Problematic

The issues introduced by embedded scripting are not immediately obvious during development but become severe under production load. They fall into four key categories:

### Performance Bottleneck

GraalJS operates in interpreted mode by default, meaning the JVM continuously recompiles script code on every execution rather than optimising it. This causes CPU spikes and throughput degradation under load.

When Interlok invokes an `embedded-scripting-service`, the GraalJS polyglot engine must parse and interpret the script on each execution. Unlike JIT compiled Java code, the script does not benefit from runtime optimisation. In high traffic workflows where a service may be invoked thousands of times per minute, this results in:

* Sustained CPU utilisation well above baseline
* Increased latency per message processed
* Reduced overall workflow throughput
* Contention in thread pools due to the polyglot engine's synchronisation overhead

### Memory Pressure and Heap Degradation

Heavy use of `JSON.parse()` and `JSON.stringify()` on large payloads generates extreme object churn. The Garbage Collector struggles to reclaim these short lived objects, leading to heap exhaustion and pod restarts.

A common pattern in embedded scripts is to deserialise a JSON payload, manipulate it in memory, and re serialise it. Each call to `JSON.parse()` allocates a new object graph on the JVM heap. In high throughput scenarios, these objects are created faster than the Garbage Collector can reclaim them, leading to:

* Rapid heap growth that appears superficially similar to a memory leak
* Frequent and increasingly long GC pause cycles
* `OutOfMemoryError` exceptions causing container restarts
* Cascading instability in downstream services if the pod crashes mid workflow

> **Diagnosis Tip**
>
> Heap growth caused by scripting object churn is often misdiagnosed as a traditional memory leak. Before assuming a leak, profile the heap to check for excessive short lived object allocation from the scripting engine. Replacing the script with a native service is frequently the complete resolution.

### Security Vulnerabilities

Embedded scripts frequently rely on specific versions of transitive dependencies (for example `jackson-databind`, `httpcore`) that may be flagged by vulnerability scans, accumulating technical debt over time.

Embedded scripts that interact with Java types directly (for example via `Java.type()` in GraalJS) may depend on specific internal library versions. When those libraries are flagged by CVE scanners, upgrading them can be blocked by the script's implicit dependency on their APIs, creating a maintenance burden and leaving known vulnerabilities unpatched longer than necessary.

### Operational Complexity

Native Interlok services are declarative, easier to audit, and integrate cleanly with configuration based health checks and observability pipelines. Scripts are opaque to standard Interlok monitoring and configuration tooling.

---

## Migration Examples

The following examples demonstrate real world replacements of embedded scripts with equivalent native Interlok services. In each case, the native implementation is more performant, more readable, and easier to maintain.

### Example 1 - JSON Payload Transformation

A common use case is transforming a JSON array returned from a database query: parsing nested string fields, reshaping the structure, and extracting metadata such as record count. The script below performs this using JavaScript's `JSON.parse()` and `Array.map()`, which when executed against large result sets at high frequency generates significant heap pressure.

The replacement uses `json-jq-transform`, which processes the payload natively in Java using a compiled JQ expression, with no intermediate object graph allocation on the scripting engine's heap.

#### Before - embedded-scripting-service

```xml
<embedded-scripting-service>
  <unique-id>transform-db-result-set</unique-id>
  <language>javascript</language>
  <script>
var payloadString = message.getContent();
var rootJson = JSON.parse(payloadString);

var result = rootJson.map(function(item) {
  return {
    recordId: item.recordId,
    accountId: item.accountId,
    version: item.version,
    payload: JSON.parse(item.payload)
  };
});

message.addMetadata("resultCount", result.length);
message.setContent(
  JSON.stringify(result),
  message.getContentEncoding()
);
  </script>
</embedded-scripting-service>
```

### After - json-jq-transform

```xml
<json-jq-transform>
  <unique-id>transform-db-result-set</unique-id>
  <query-source class="constant-data-input-parameter">
    <value>
map({
  recordId: .recordId,
  accountId: .accountId,
  version: .version,
  payload: (.payload | fromjson)
})
    </value>
  </query-source>
  <query-target class="string-payload-data-input-parameter"/>
  <output-target class="string-payload-data-output-parameter"/>
</json-jq-transform>
```

> **Note on Record Count Extraction**
> 
> The original script also extracted the array length into metadata. After migrating the transformation to json-jq-transform, use a separate json-path-service with the expression $.length() to write the count to a metadata key. Validate this expression carefully. $.length (without parentheses) will not work on array roots in all implementations.

### Example 2 - HMAC Authentication Hash
A second common pattern is computing a keyed hash (for example HmacMD5) for authentication headers. The embedded script below uses Java.type() to access the JCE API directly, coupling the script to internal Java class paths and requiring careful management of the polyglot security context.

The metadata-hashing-service provides an identical capability declaratively, with no scripting overhead, no polyglot engine involvement, and full compatibility with Interlok's configuration driven monitoring.

### Before - embedded-scripting-service
```xml
<embedded-scripting-service>
  <unique-id>compute-auth-hash</unique-id>
  <language>javascript</language>
  <script>
var MessageDigest = Java.type('javax.crypto.Mac');
var SecretKeySpec = Java.type('javax.crypto.spec.SecretKeySpec');
var Base64 = Java.type('java.util.Base64');

var password = message.getMetadataValue("authPassword");
var stringToHash = message.getMetadataValue("authInput");

var mac = MessageDigest.getInstance("HmacMD5");
var key = new SecretKeySpec(
  password.getBytes(), 0,
  password.length(), "HmacMD5"
);
mac.init(key);
var hash = Base64.getEncoder()
  .encodeToString(
    mac.doFinal(stringToHash.getBytes())
  );

message.addMetadata("authHash", hash);
  </script>
</embedded-scripting-service>
```

### After - metadata-hashing-service
```xml
<metadata-hashing-service>
  <unique-id>compute-auth-hash</unique-id>

  <!-- Key to write the hash result into -->
  <metadata-key-regexp>authHash</metadata-key-regexp>

  <!-- Algorithm matches the original script -->
  <hash-algorithm>HmacMD5</hash-algorithm>

  <!-- Base64 encoding matches original -->
  <byte-translator class="base64-byte-translator"/>

  <!-- HMAC key sourced from metadata -->
  <hmac-key>%message{authPassword}</hmac-key>
</metadata-hashing-service>

<!-- The authInput metadata value is
     consumed automatically as the
     input to the hash function -->
```

> **Benefits of the Native Service**
>
> The metadata-hashing-service executes entirely within the JVM without invoking the polyglot engine. It is fully declarative, auditable in configuration management, and does not require granting the scripting context access to JCE internals via Java.type().

### When to Use Embedded Scripts
Use the following framework to guide your decision. The default position should always be to reach for a native service first.

| Use Case | Recommendation | Native Alternative|
| -------- |----------------|-------------------|
| JSON payload reshaping / field extraction | Use Native | json-jq-transform, json-path-service |
| HMAC / cryptographic hashing | Use Native | metadata-hashing-service |
| XML transformation | Use Native | xslt-service |
| Metadata manipulation / string operations | Use Native | add-metadata-service, metadata-value-branching-service |
| HTTP / REST calls | Use Native | apache-http-producer, standard-http-producer |
| Complex conditional branching logic | Evaluate | Consider branching-service-collection with expressions |
| Highly bespoke algorithm with no native equivalent | Acceptable | Consider writing a custom Java service instead |
| Rapid prototyping / local development only | Temporary | Replace before promoting to production |
| High throughput production workflow | Avoid | Any native service equivalent |
| Long running / always on deployment | Avoid | Any native service equivalent |

> **Custom Java Services**
>
> If no native service exists for your use case and the logic is complex enough to warrant it, the preferred alternative to an embedded script is a custom Java service compiled against the Interlok API. This runs at full JVM speed, benefits from JIT compilation, and integrates cleanly with the component lifecycle.

### Garbage Collection Considerations
If embedded scripts cannot be immediately replaced and you are experiencing heap pressure, Garbage Collector configuration can provide short term relief. However, this should be treated as a temporary mitigation, not a solution.

**G1GC - Use with Caution on Constrained Pods**
* Designed for multi core, larger heap environments
* On pods with limited CPU (for example 250m to 500m), G1GC's concurrent threads compete with application threads
* Can cause synchronisation bottlenecks that worsen performance under scripting load
* Not recommended for "micro" pod configurations

**SerialGC - Recommended for Constrained Pods**
* Single threaded collector with no concurrent overhead
* More predictable pause behaviour on low CPU pods
* Avoids the multi threaded synchronisation issues that cause G1GC to stall
* Enable with -XX:+UseSerialGC

**Additional JVM Flags**
* GC Logging: Use -Xlog:gc=warning:stderr to capture meaningful GC events without flooding logs with routine output.
* Avoid panic flags: Do not use -XX:GCTimeLimit or -XX:GCHeapFreeLimit in production. These can trigger premature OutOfMemoryError throws during legitimate GC cycles under load, causing unnecessary pod restarts.
* Resource consistency: Set Kubernetes resource requests and limits to the same value to prevent CPU throttling, which can cause GC pauses to appear much longer than they are.

> GC Tuning is a Mitigation, Not a Fix
>
> Adjusting GC settings can reduce the frequency of crashes caused by scripting induced heap pressure, but it does not eliminate the root cause. The only durable fix is to replace embedded scripts with native services.

### Migration Checklist
Use this checklist when auditing an existing Interlok configuration for embedded scripting usage:

**Do This**
- [ ] Audit all workflows for <embedded-scripting-service> elements. Treat each occurrence as a candidate for replacement.
- [ ] Identify the logical intent of each script (transformation, hashing, branching, etc.) and map it to the most appropriate native service.
- [ ] Validate JSON path expressions carefully when migrating. Use $.length() (with parentheses) for array length on root arrays; $.length will not work in all implementations.
- [ ] Profile heap usage before and after migration using a local heap dump or JVM profiler to confirm the object churn has been eliminated.
- [ ] Review dependency versions after removing scripting services. Dependencies previously pinned to support script behaviour may now be safely upgraded, resolving outstanding CVEs.
- [ ] Run load tests against the migrated configuration before promoting to production to confirm throughput and memory stability improvements.

**Don't Do This**
- [ ] Do not promote configurations containing embedded scripts to production without explicit justification and sign off that no native equivalent exists.
- [ ] Do not use -XX:GCTimeLimit or -XX:GCHeapFreeLimit as a substitute for addressing scripting induced memory pressure.
- [ ] Do not assume heap growth is a traditional memory leak before ruling out scripting object churn. Profile first.

### Key Takeaways
1. Embedded scripts are a performance and stability risk in high throughput and long running deployments due to interpreter overhead and object churn.
2. Always prefer native services when available. They are declarative, auditable, performant, and integrate seamlessly with Interlok's configuration and monitoring ecosystem.
3. Memory leaks are often misdiagnosed object churn from scripting. Profile heap allocation before assuming a traditional leak.
4. Garbage Collector tuning is temporary relief, not a permanent fix. The durable solution is replacing scripts with native services.
5. Audit existing configurations for embedded scripting and migrate them systematically, validating with load tests before production deployment.