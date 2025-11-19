# Interlok AWS SQS (SDK v2)

Interlok AWS SQS provides integration with Amazon Simple Queue Service (SQS) for sending and receiving messages. This version uses **AWS SDK v2**.

> **Note:** This is the AWS SDK v2 implementation. For the SDK v1 version, see [interlok-aws-sqs](../interlok-aws-sqs/).

## Overview

The `interlok-aws2-sqs` component provides consumer and producer functionality for Amazon SQS using AWS SDK v2, enabling reliable message queuing with improved performance and modern API design.

**Key Features:**
- Consume messages from SQS queues
- Produce messages to SQS queues
- Support for message attributes
- Configurable visibility timeout
- Dead letter queue support
- Built on AWS SDK v2 for better performance

## Installation

```xml
<dependency>
  <groupId>com.adaptris</groupId>
  <artifactId>interlok-aws2-sqs</artifactId>
  <version>4.x.x</version>
</dependency>
```

## SDK v2 Advantages

- **Better Performance**: Improved HTTP client with connection pooling
- **Smaller Footprint**: Reduced dependency size
- **Modern API**: Cleaner, more intuitive design
- **Active Development**: AWS focuses on SDK v2

## Quick Start

### SQS Consumer

```xml
<consumer class="aws2-sqs-consumer">
  <connection class="aws2-sqs-connection">
    <region>us-east-1</region>
    <credentials class="aws2-default-credentials-provider"/>
  </connection>
  <queue>my-queue</queue>
  <max-messages>10</max-messages>
  <visibility-timeout>30</visibility-timeout>
  <wait-time>20</wait-time>
</consumer>
```

### SQS Producer

```xml
<producer class="aws2-sqs-producer">
  <connection class="aws2-sqs-connection">
    <region>us-east-1</region>
    <credentials class="aws2-default-credentials-provider"/>
  </connection>
  <queue>my-queue</queue>
  <message-attributes>
    <key-value-pair>
      <key>priority</key>
      <value>high</value>
    </key-value-pair>
  </message-attributes>
</producer>
```

### With Message Delay

```xml
<producer class="aws2-sqs-producer">
  <connection class="aws2-sqs-connection">
    <region>us-east-1</region>
    <credentials class="aws2-default-credentials-provider"/>
  </connection>
  <queue>my-queue</queue>
  <delay-seconds>60</delay-seconds>
</producer>
```

### LocalStack Testing

```xml
<connection class="aws2-sqs-connection">
  <region>us-east-1</region>
  <credentials class="aws2-static-credentials-builder">
    <access-key>test</access-key>
    <secret-key>test</secret-key>
  </credentials>
  <endpoint-override>http://localhost:4566</endpoint-override>
</connection>
```

## Configuration Reference

For detailed configuration including:
- Connection properties
- Consumer configuration (polling, visibility timeout, message deletion)
- Producer configuration (message attributes, delay)
- Queue URL vs queue name
- FIFO queue support
- Best practices
- Troubleshooting

Please refer to the [interlok-aws-sqs documentation](../interlok-aws-sqs/), as the configuration is nearly identical between SDK v1 and v2 versions.

## Key Differences from SDK v1

1. **Artifact**: `interlok-aws-sqs` → `interlok-aws2-sqs`
2. **Connection Class**: `aws-sqs-connection` → `aws2-sqs-connection`
3. **Consumer Class**: `aws-sqs-consumer` → `aws2-sqs-consumer`
4. **Producer Class**: `aws-sqs-producer` → `aws2-sqs-producer`
5. **Credentials**: Use `aws2-*-credentials-builder` classes
6. **Endpoint**: `endpoint-override` instead of `custom-endpoint`

## Additional Resources

- [AWS SQS Documentation](https://docs.aws.amazon.com/sqs/latest/dg/welcome.html)
- [AWS SDK for Java 2.x](https://docs.aws.amazon.com/sdk-for-java/latest/developer-guide/home.html)
- [Interlok AWS SQS (SDK v1)](../interlok-aws-sqs/)
- [Interlok Documentation](https://interlok.adaptris.net/)

## License

This component is licensed under the Apache License 2.0.
