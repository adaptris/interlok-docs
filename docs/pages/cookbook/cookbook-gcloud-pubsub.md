# Integrating with Google Cloud Pub\/Sub

> **Summary:** This document summarises configurations for consuming and producing messages using Google Cloud Pub\/Sub. It assumes a passing knowledge of Interlok and its configuration with a basic understanding of Google Cloud Pub\/Sub concepts.

!> **IMPORTANT:** Ensure you have the Interlok Google Cloud Pub\/Sub subcomponent installed and the Google Cloud client libraries available to your Interlok installation. The examples below describe generic Interlok configuration patterns and may need minor adaptation for specific Interlok component names/versions. See the JavaDocs for full configuration details: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-gcloud-pubsub/

## Getting Started ##

### Interlok Pre-requisites ###

Before starting Interlok that will consume or produce messages to Google Cloud Pub\/Sub:

- Install the Interlok Google Cloud Pub\/Sub subcomponent (copy the component JARs into the `lib` directory or install via your distribution mechanism).
- Ensure Google Cloud client libraries are available to Interlok if not bundled with the subcomponent.
- Create a Google Cloud service account with the minimum IAM roles (`pubsub.publisher` and/or `pubsub.subscriber`) and download the service account key JSON.
- Provide credentials to Interlok by either:
    - setting the environment variable `GOOGLE_APPLICATION_CREDENTIALS` to the service account JSON path; or
    - configuring credentials explicitly on the Pub\/Sub connection component.
- Enable the Pub\/Sub API in your Google Cloud project.

### Google Cloud Pub\/Sub basics ###

- Topic: named resource to which messages are published.
- Subscription: named resource representing a stream of messages from a topic.
- Pull vs Push subscriptions: Pull subscribers request messages; Push subscribers receive HTTP(S) pushes.
- Acknowledge semantics: subscribers must acknowledge messages (enabled by default in interlok); unacked messages are redelivered.
- Ordering keys: optional keys preserving ordering for messages with the same key.
- Dead-letter topics: supported to handle poison messages\/retries.

Addressing formats:

- `projects/{project-id}/topics/{topic-name}`
- `projects/{project-id}/subscriptions/{subscription-name}`

----

## Interlok Configuration ##

A common loopback test uses two channels: one that reads files and publishes to a Pub\/Sub topic (producer), and one that pulls messages from a subscription and writes them to the filesystem (consumer). Both components require a Pub\/Sub connection with fields described below.

Core connection fields (typical):

- `project-id` \- the Google Cloud project id.
- `credentials` \- path to service account JSON or use application-default credentials.
- `endpoint` \- optional; set to the Pub\/Sub emulator endpoint for local testing.
- `timeout` / `transport-settings` \- optional network/timeouts (component-specific).

Addressing:

- Producer topic: `projects/{project-id}/topics/{topic-name}`
- Consumer subscription: `projects/{project-id}/subscriptions/{subscription-name}`

Message translation:

- `byte-translator` \- how to translate AdaptrisMessage payload to\/from bytes (UTF-8 text vs raw bytes).
- `message-attributes-mappers` \- map AdaptrisMessage metadata and ids to Pub\/Sub attributes and vice versa.

### Producers & Consumers ###

Producer and consumer components expose configuration for batching, flow control, acknowledgement behaviour and attribute mapping. Common fields include:

| Field | Description |
|----|-----------|
| `project-id` | Google Cloud project id |
| `credentials` | Path or reference to service account JSON / ADC |
| `topic` | Full topic name for producers |
| `subscription` | Full subscription name for consumers |
| `endpoint` | Optional emulator or custom endpoint |
| `batching-config` | Producer batching: maxMessages, maxBytes, delayThreshold (tune for throughput) |
| `flow-control` | Consumer flow control: maxOutstandingMessages, maxOutstandingBytes |
| `ordering-key` | Optional: ordering key for published messages |
| `ack-deadline` | Consumer ack deadline; may be extended by processing code |
| `dead-letter-topic` | Optional DLQ topic for failed messages / retries |
| `message-attributes-mappers` | Mappers to map AdaptrisMessage metadata\/payload to Pub\/Sub attributes |
| `byte-translator` | How to translate AdaptrisMessage payload to\/from bytes |

Mapping responsibilities:

- map an AdaptrisMessage unique id to a Pub\/Sub attribute
- map metadata entries to Pub\/Sub attributes and vice-versa
- control whether payload is treated as UTF\-8 text or raw bytes

Property mappers (typical implementations):

- configured attribute mapper \- map literal values to attributes
- message id mapper \- map AdaptrisMessage unique id to\/from attribute
- metadata mapper \- map metadata keys to attributes
- xpath mapper \- resolve XPath against XML payload and set attribute

Note: Pub\/Sub message payload is binary; configure `byte-translator` appropriately. By default, treat payload as UTF\-8 for text messages.

----

## Best Practices ##

- Use least-privilege service accounts. Grant only `pubsub.publisher`, `pubsub.subscriber` as needed.
- Use batching on producers to increase throughput; tune `maxMessages`, `maxBytes`, `delayThreshold`.
- Use flow control on consumers to avoid memory pressure.
- Use dead-letter topics and retry policies for poison messages rather than tight retry loops.
- Extend ack deadline only while actively processing long-running messages; otherwise ack promptly.
- Prefer Pull subscriptions for server-side processing.
- Use ordering keys only when strict ordering per key is required; expect throughput trade-offs.
- For local development use the Pub\/Sub emulator and configure the connection `endpoint`.
- Monitor metrics (ack rates, processing latency, backlog) and set alerts for unusual backlog growth.

----

## Examples ##

### Example Connection
The example connection includes a configurable `credentials-provider`. This controls how the Google Cloud client obtains credentials used to access Pub\/Sub.
```xml
<google-cloud-pubsub-connection>
    <connection-error-handler class="google-cloud-pubsub-connection-error-handler"/>
    <unique-id>gcloud-pubsub-connection</unique-id>
    <credentials-provider class="no-credentials-provider"/>
    <channel-provider class="default-channel-provider"/>
    <flow-control-provider class="default-flow-control-provider"/>
    <project-name>test-project</project-name>
</google-cloud-pubsub-connection>
```
#### Credentials
You can supply credentials via the environment (Application Default Credentials), point to a service-account key file, or use a no-op provider for local emulator/testing.

Common provider options (actual class names may vary by Interlok distribution):

- `no-credentials-provider` \- use when the Pub\/Sub emulator is used or when no credentials are required.
- `file-credentials-provider` \- load a service account JSON key file; configure the key file path on the provider.
- `application-default-credentials-provider` \- use Application Default Credentials (ADC); useful when running on GCP or when `GOOGLE_APPLICATION_CREDENTIALS` is set.

Notes:
- If using ADC, set the environment variable `GOOGLE_APPLICATION_CREDENTIALS` to the JSON key path or rely on platform-provided credentials.
- For local development with the Pub\/Sub emulator, set the connection's `endpoint` and typically use `no-credentials-provider`.
- Always prefer least-privilege service accounts with the minimal `pubsub.publisher` / `pubsub.subscriber` roles.

XML example (credentials file provider):
```xml
<google-cloud-pubsub-connection>
    <unique-id>gcloud-pubsub-connection</unique-id>
    <credentials-provider class="file-credentials-provider">
        <credentials-file>C:\path\to\service-account.json</credentials-file>
    </credentials-provider>
    <project-name>test-project</project-name>
</google-cloud-pubsub-connection>
```

### Example Consumer
By default, the pull consumer has `auto-acknowledge` and `create-subscription` set to `true`. This causes Interlok to automatically create the subscription if missing and to acknowledge messages after successful processing. Set these fields explicitly to change behaviour (for example, use `auto-acknowledge = false` for manual acknowledgement or `create-subscription = false` to manage subscriptions externally).
```xml
<consumer class="google-cloud-pubsub-pull-consumer">
    <unique-id>pubsub-consumer</unique-id>
    <subscription-name>test-sub</subscription-name>
    <ack-deadline>
        <unit>SECONDS</unit>
        <interval>10</interval>
    </ack-deadline>
    <create-subscription>true</create-subscription>
    <auto-acknowledge>true</auto-acknowledge>
    <topic>test-topic</topic>
</consumer>
```

### Example Producer
The example producer publishes payloads to the configured Pub/Sub topic, using the connection's credentials.
```xml
<producer class="google-cloud-pubsub-producer">
    <unique-id>pubsub-producer</unique-id>
    <topic>test-topic</topic>
</producer>
```

----

## Useful Links ##

- Google Cloud Pub\/Sub documentation: https://cloud.google.com/pubsub/docs
- Pub\/Sub emulator: https://cloud.google.com/pubsub/docs/emulator
- Pub\/Sub best practices: https://cloud.google.com/pubsub/docs/best-practices
- IAM and service accounts: https://cloud.google.com/iam/docs
- Interlok Google Cloud Pub\/Sub JavaDocs: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-gcloud-pubsub/
