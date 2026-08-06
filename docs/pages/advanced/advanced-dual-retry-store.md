## Introduction

Handling failed messages is a critical aspect of any enterprise messaging system. Sometimes a single retry store isn't enough—your application might need to route failed messages to different stores based on business logic, geographic regions, or data routing requirements. This is where `RetryFromJettyDualStore` comes in.

`RetryFromJettyDualStore` is a powerful implementation of the `FailedMessageRetrier` interface that enables you to manage failed messages across **two distinct retry stores** with intelligent routing. This tutorial will guide you through understanding its capabilities, configuring it via XStream XML, and implementing best practices.

## What is RetryFromJettyDualStore?

`RetryFromJettyDualStore` is a Jetty-based failed message retrier that:

- **Listens on HTTP endpoints** for retry requests
- **Manages two separate retry stores** (primary and secondary)
- **Routes requests by region in the URL path** with optional expression fallback
- **Provides RESTful operations** for listing, retrying, deleting, and inspecting failed messages

It extends `RetryFromJettyBase`, inheriting lifecycle and retry-store handling while adding dual-store support with region path-based routing.

### Key Characteristics

| Feature | Description |
|---------|-------------|
| **Dual Stores** | Maintains and manages two independent `RetryStore` instances |
| **Path-Based Routing** | Uses the `{region}` path segment to determine which store to use |
| **RESTful Interface** | HTTP endpoints for listing, retrying, deleting messages, and retrieving stack traces |
| **Safe Resolution** | Route is resolved from URL path first, then optional expression fallback; unknown path regions return HTTP 404, while unresolved metadata/expression routes return HTTP 400 |
| **Available Since** | Interlok 5.0.6 |

## XStream XML Configuration

The `@XStreamAlias` annotation maps `RetryFromJettyDualStore` to the XML element `retry-via-jetty-dual-store`.

### Basic Configuration Structure

```xml
<retry-via-jetty-dual-store>
    <!-- HTTP Endpoints are region-aware by default -->
    <!-- /api/{region}/retry/{msgId} -->
    <!-- /api/failed/{region}/list -->
    <!-- /api/failed/{region}/delete/{msgId} -->
    <!-- /api/failed/{region}/stacktrace/{msgId} -->
    
    <!-- Connection (defaults to EmbeddedConnection) -->
    <connection class="com.adaptris.core.http.jetty.EmbeddedConnection">
        <port>8080</port>
    </connection>
    
    <!-- First Retry Store Configuration -->
    <first-retry-store>
        <!-- Configured with your chosen RetryStore implementation (e.g., JdbcFailedMessageStore) -->
    </first-retry-store>
    <first-retry-store-identifier>usa</first-retry-store-identifier>
    
    <!-- Second Retry Store Configuration -->
    <second-retry-store>
        <!-- Configured with your chosen RetryStore implementation -->
    </second-retry-store>
    <second-retry-store-identifier>eu</second-retry-store-identifier>
    
    <!-- Routing Expression (optional fallback if region is not in URL path) -->
    <retry-store-routing-expression>%message{routing.region}</retry-store-routing-expression>
    
    <!-- Report Builder (optional) -->
    <report-builder class="com.adaptris.core.http.jetty.retry.ReportBuilder" />
    
    <!-- HTTP Methods (optional, uses defaults if not specified) -->
    <retry-http-method>POST</retry-http-method>
    <delete-http-method>DELETE</delete-http-method>
    <stack-trace-http-method>GET</stack-trace-http-method>
</retry-via-jetty-dual-store>
```

## Understanding the Core Configuration Elements

### 1. Retry Stores

The first and second retry stores are where your failed messages are persisted. They must be distinct `RetryStore` implementations:

```xml
<first-retry-store class="com.adaptris.core.services.jdbc.JdbcFailedMessageStore">
    <connection class="com.adaptris.core.http.jetty.JettyConnection">
        <!-- Database configuration -->
    </connection>
    <tablename>failed_messages_usa</tablename>
</first-retry-store>

<second-retry-store class="com.adaptris.core.services.jdbc.JdbcFailedMessageStore">
    <connection class="com.adaptris.core.http.jetty.JettyConnection">
        <!-- Database configuration -->
    </connection>
    <tablename>failed_messages_eu</tablename>
</second-retry-store>
```

### 2. Store Identifiers

Store identifiers are normalized (lowercased) strings that uniquely identify each store. They are used to match against the routing expression result:

```xml
<first-retry-store-identifier>usa</first-retry-store-identifier>
<second-retry-store-identifier>eu</second-retry-store-identifier>
```

**Important**: These identifiers must be **distinct** and cannot be the same. They can be either static strings or message expressions (e.g., `%message{store-id}`).

### 3. Retry Store Routing Expression (Optional Fallback)

Primary routing uses the region in the URL path. `retry-store-routing-expression` is an optional fallback only when the region is unavailable from the path:

```xml
<retry-store-routing-expression>%message{routing.region}</retry-store-routing-expression>
```

In this example:
- If URL path contains `/.../usa/...` → routes to the first store
- If URL path contains `/.../eu/...` → routes to the second store
- If path region is missing and expression resolves to `usa` or `eu` → routes accordingly
- If the path contains an unknown region → request is rejected with HTTP 404
- If neither path nor expression resolves to a configured store → request is rejected with HTTP 400

The routing expression can be as simple or complex as needed:

```xml
<!-- Simple metadata lookup -->
<retry-store-routing-expression>%message{region}</retry-store-routing-expression>

<!-- Dynamic expression with conditional logic -->
<retry-store-routing-expression>
    %message{header.destination-region}
</retry-store-routing-expression>

<!-- Expression using XPath (if message contains XML) -->
<retry-store-routing-expression>
    %xpath{/request/region/text()}
</retry-store-routing-expression>
```

## HTTP Endpoints Reference

`RetryFromJettyDualStore` exposes four main RESTful endpoints (using default paths):

### 1. List Failed Messages
```bash
curl -XGET http://localhost:8080/api/failed/{region}/list
```
- **Method**: GET (configurable)
- **Returns**: HTTP 200 with a list of failed message IDs from the resolved store
- **Returns**: HTTP 404 if the path contains an unknown region; HTTP 400 if routing cannot be resolved

### 2. Retry a Message
```bash
curl -XPOST http://localhost:8080/api/{region}/retry/{msgId}
```
- **Method**: POST (configurable)
- **Returns**: HTTP 202 (Accepted) if successful
- **Returns**: HTTP 404 if the path contains an unknown region; HTTP 400 if routing cannot be resolved or message ID is invalid
- **Behavior**: Resubmits the message to the workflow; returns immediately

### 3. Delete a Message
```bash
curl -XDELETE http://localhost:8080/api/failed/{region}/delete/{msgId}
```
- **Method**: DELETE (configurable)
- **Returns**: HTTP 200 if deleted successfully
- **Returns**: HTTP 404 if message not found
- **Returns**: HTTP 404 if the path contains an unknown region; HTTP 400 if routing cannot be resolved

### 4. Get Stack Trace
```bash
curl -XGET http://localhost:8080/api/failed/{region}/stacktrace/{msgId}
```
- **Method**: GET (configurable)
- **Returns**: HTTP 200 with stack trace if found
- **Returns**: HTTP 404 if the path contains an unknown region; HTTP 400 if routing cannot be resolved or message ID is invalid

## Complete Configuration Example

Here's a practical example with S3-based retry stores:

```xml
<retry-via-jetty-dual-store>
    <!-- Jetty Connection -->
    <connection class="com.adaptris.core.http.jetty.EmbeddedConnection">
        <port>8080</port>
        <bind-address>0.0.0.0</bind-address>
    </connection>
    
    <!-- Primary (USA Region) Retry Store -->
    <first-retry-store 
        class="com.adaptris.core.services.s3.S3FailedMessageStore">
        <connection class="com.adaptris.aws.s3.AmazonS3Connection">
            <access-key>${aws.access-key}</access-key>
            <secret-key>${aws.secret-key}</secret-key>
            <region>us-east-1</region>
        </connection>
        <bucket-name>failed-messages-usa</bucket-name>
        <key-prefix>retry/</key-prefix>
    </first-retry-store>
    <first-retry-store-identifier>usa</first-retry-store-identifier>
    
    <!-- Secondary (EU Region) Retry Store -->
    <second-retry-store 
        class="com.adaptris.core.services.s3.S3FailedMessageStore">
        <connection class="com.adaptris.aws.s3.AmazonS3Connection">
            <access-key>${aws.eu-access-key}</access-key>
            <secret-key>${aws.eu-secret-key}</secret-key>
            <region>eu-west-1</region>
        </connection>
        <bucket-name>failed-messages-eu</bucket-name>
        <key-prefix>retry/</key-prefix>
    </second-retry-store>
    <second-retry-store-identifier>eu</second-retry-store-identifier>
    
    <!-- Routing Expression (optional fallback) -->
    <retry-store-routing-expression>%message{deployment.region}</retry-store-routing-expression>
    
    <!-- Custom HTTP Methods -->
    <retry-http-method>POST</retry-http-method>
    <delete-http-method>DELETE</delete-http-method>
    <stack-trace-http-method>GET</stack-trace-http-method>
    
    <!-- Report Builder -->
    <report-builder class="com.adaptris.core.http.jetty.retry.ReportBuilder">
        <!-- Optional report builder configuration -->
    </report-builder>
</retry-via-jetty-dual-store>
```

## Configuration Validation

`RetryFromJettyDualStore` performs strict validation during the `prepare()` lifecycle phase:

| Validation | Error Message |
|-----------|---------------|
| First store is not configured | "No first RetryStore configured; configure firstRetryStore." |
| Second store is not configured | "No second RetryStore configured; configure secondRetryStore." |
| Routing expression is blank | Allowed (path-based routing still works) |
| Store identifiers are blank | "firstRetryStoreIdentifier and secondRetryStoreIdentifier are required." |
| Store identifiers are identical | "firstRetryStoreIdentifier and secondRetryStoreIdentifier must be distinct." |

## Best Practices

### 1. Choose Store Identifiers Wisely

Use clear, unambiguous identifiers that map directly to your business logic:

```xml
<!-- Good: Clear region identifiers -->
<first-retry-store-identifier>primary-region</first-retry-store-identifier>
<second-retry-store-identifier>secondary-region</second-retry-store-identifier>

<!-- Good: Geographic identifiers -->
<first-retry-store-identifier>apac</first-retry-store-identifier>
<second-retry-store-identifier>emea</second-retry-store-identifier>

<!-- Avoid: Generic or confusing names -->
<first-retry-store-identifier>store1</first-retry-store-identifier>
<second-retry-store-identifier>store2</second-retry-store-identifier>
```

### 2. Ensure Routing Resolution Reliability

Your URL path region must resolve to one of your configured identifiers. If your path region is unavailable, the optional fallback expression must resolve to one of your configured identifiers. Unknown path regions result in HTTP 404 errors; unresolved metadata/expression routes result in HTTP 400 errors:

```xml
<!-- Ensure the metadata key exists and maps to valid identifiers -->
<retry-store-routing-expression>
    %message{routing.destination}
</retry-store-routing-expression>

<!-- Consider case normalization in your message processing -->
<!-- Routing expressions are normalized to lowercase automatically -->
```

### 3. Use Expression Hints for Dynamic Identifiers

If your identifiers are expressions themselves, annotate them appropriately:

```xml
<!-- Static identifier -->
<first-retry-store-identifier>usa</first-retry-store-identifier>

<!-- Dynamic identifier via expression -->
<first-retry-store-identifier>%message{store-id}</first-retry-store-identifier>
```

### 4. Monitor HTTP Response Codes

Understand what each HTTP response code means:
- **200 OK**: Operation successful (list, delete, or stacktrace)
- **202 Accepted**: Retry submitted successfully
- **400 Bad Request**: Invalid request or routing resolution failed
- **404 Not Found**: Message ID not found in store
- **500 Internal Server Error**: Unexpected exception

### 5. Implement Proper Error Handling

Since unresolved metadata/expression routes return HTTP 400, implement client-side retry logic with proper exponential backoff:

```bash
#!/bin/bash
MAX_RETRIES=3
RETRY_DELAY=2

for attempt in $(seq 1 $MAX_RETRIES); do
    response=$(curl -s -w "%{http_code}" -XPOST \
        "http://localhost:8080/api/usa/retry/MSG-12345")
    
    if [[ ${response: -3} == "202" ]]; then
        echo "Retry successful"
        exit 0
    fi
    
    if [[ $attempt -lt $MAX_RETRIES ]]; then
        sleep $((RETRY_DELAY * attempt))
    fi
done
```

### 6. Isolate Stores by Deployment Context

Use separate databases or storage buckets for each store to prevent cross-contamination:

```xml
<!-- Separate S3 buckets by region -->
<first-retry-store class="com.adaptris.core.services.s3.S3FailedMessageStore">
    <bucket-name>failed-messages-us-east-1</bucket-name>
</first-retry-store>

<second-retry-store class="com.adaptris.core.services.s3.S3FailedMessageStore">
    <bucket-name>failed-messages-eu-west-1</bucket-name>
</second-retry-store>
```

### 7. Plan for Future Scaling

While `RetryFromJettyDualStore` manages exactly two stores, design your routing logic to be extensible. If you anticipate needing more than two stores in the future, consider:
- Using a generic routing metadata field that references store names
- Implementing a separate routing service layer
- Planning a migration path to a future multi-store implementation

### 8. Document Your Routing Rules

Create clear documentation for your operational teams:

```xml
<!--
Routing Rules:
- Messages from USA deployments (deployment.region="USA") → first store (S3 us-east-1)
- Messages from EU deployments (deployment.region="EU") → second store (S3 eu-west-1)
- Unrecognized path regions result in HTTP 404 errors
- Store identifiers are case-insensitive (automatically normalized to lowercase)
-->
```

## Comparison with RetryFromJetty

`RetryFromJetty` is the single-store predecessor to `RetryFromJettyDualStore`:

| Feature | RetryFromJetty | RetryFromJettyDualStore |
|---------|---|---|
| Number of Stores | 1 | 2 |
| Routing Logic | None (direct) | Region path-based (+ optional expression fallback) |
| Configuration | Simple | Path-based by default; optional routing expression fallback |
| Multi-Region Support | No | Yes |
| API Complexity | Low | Medium |
| Use Case | Single store scenarios | Multi-region/multi-store scenarios |

Use `RetryFromJettyDualStore` when you need message routing logic; otherwise, `RetryFromJetty` is simpler and sufficient.

## Troubleshooting

### Issue: All Requests Return HTTP 404

**Cause**: The URL path contains a region that does not match either configured store identifier.

**Solution**:
```xml
<!-- Verify the request path uses one of the configured region identifiers -->
<!-- Example: /api/failed/usa/list or /api/failed/eu/list -->
```

### Issue: All Requests Return HTTP 400

**Cause**: Region could not be resolved from path or fallback expression.

**Solution**:
```xml
<!-- Debug by adding logging -->
<!-- Check that the metadata key exists in your messages -->
<!-- Verify the resolved value matches one of your store identifiers -->
<retry-store-routing-expression>%message{routing.region}</retry-store-routing-expression>
```

### Issue: Messages Appearing in Wrong Store

**Cause**: Routing expression or message metadata is incorrect.

**Solution**:
- Verify store identifiers are case-insensitive and normalized
- Check that incoming requests use the correct `{region}` path segment
- If relying on fallback, check that routing metadata is set correctly
- Use logging/debugging to inspect expression resolution

### Issue: HTTP 404 When Retrying Messages

**Cause**: Message ID doesn't exist in the resolved store.

**Solution**:
- Verify the message was actually stored in that specific store
- Check that the routing logic produces the same result as when the message failed
- Investigate if the message has been deleted or expired

## Lifecycle Management

`RetryFromJettyDualStore` follows the standard Interlok lifecycle:

1. **prepare()** - Validates configuration and initializes infrastructure
2. **init()** - Initializes both retry stores and HTTP listeners
3. **start()** - Starts listening on configured HTTP endpoints
4. **stop()** - Stops listening (messages are not processed)
5. **close()** - Releases all resources

Both retry stores are initialized, started, stopped, and closed in parallel with the main retrier lifecycle.

## Summary

`RetryFromJettyDualStore` is a sophisticated tool for managing failed messages across multiple retry stores with intelligent routing. By understanding its configuration, endpoints, and best practices, you can build robust, geographically-distributed retry systems that handle complex enterprise messaging scenarios.

Key takeaways:
- Configure two distinct `RetryStore` instances with clear identifiers
- Route with the `{region}` URL segment; keep expression fallback optional; unknown regions return 404
- Monitor HTTP response codes for operational insights
- Document your routing rules for operational clarity
- Plan for future scalability from the start

With these principles in mind, you'll have a reliable, maintainable failed message retry system that scales with your enterprise messaging needs.

