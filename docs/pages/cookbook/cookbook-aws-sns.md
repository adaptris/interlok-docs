# Interlok AWS SNS (SDK v2)

Interlok AWS SNS provides integration with Amazon Simple Notification Service (SNS) for publishing messages to topics. This version uses **AWS SDK v2**.

> **Note:** This is the AWS SDK v2 implementation. For the SDK v1 version, see [interlok-aws-sns](../interlok-aws-sns/).

## Overview

The `interlok-aws2-sns` component provides producer functionality for Amazon SNS using AWS SDK v2, enabling you to publish messages to SNS topics with improved performance and modern API design.

**Key Features:**
- Publish messages to SNS topics
- Support for message attributes
- Subject line configuration
- Dynamic topic ARN resolution
- Built on AWS SDK v2 for better performance

## Installation

```xml
<dependency>
    <groupId>com.adaptris</groupId>
    <artifactId>interlok-aws2-sns</artifactId>
    <version>4.x.x</version>
</dependency>
```

## SDK v2 Advantages

- **Better Performance**: Improved HTTP client with connection pooling
- **Smaller Footprint**: Reduced dependency size
- **Modern API**: Cleaner, more intuitive design
- **Active Development**: AWS focuses on SDK v2

## Quick Start

### Basic SNS Producer

```xml
<producer class="aws2-sns-producer">
    <connection class="aws2-sns-connection">
        <region>us-east-1</region>
        <credentials class="aws2-default-credentials-provider"/>
    </connection>
    <topic>arn:aws:sns:us-east-1:123456789012:my-topic</topic>
    <subject>Notification from Interlok</subject>
</producer>
```

### With Message Attributes

```xml
<producer class="aws2-sns-producer">
    <connection class="aws2-sns-connection">
        <region>us-east-1</region>
        <credentials class="aws2-default-credentials-provider"/>
    </connection>
    <topic>arn:aws:sns:us-east-1:123456789012:my-topic</topic>
    <subject>%message{notificationSubject}</subject>
    <message-attributes>
        <key-value-pair>
            <key>priority</key>
            <value>high</value>
        </key-value-pair>
        <key-value-pair>
            <key>source</key>
            <value>%message{sourceSystem}</value>
        </key-value-pair>
    </message-attributes>
</producer>
```

### LocalStack Testing

```xml
<connection class="aws2-sns-connection">
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
- Producer configuration
- Message attributes
- Dynamic topic resolution
- Best practices
- Troubleshooting

Please refer to the [interlok-aws-sns documentation](../interlok-aws-sns/), as the configuration is nearly identical between SDK v1 and v2 versions.

## Key Differences from SDK v1

1. **Artifact**: `interlok-aws-sns` → `interlok-aws2-sns`
2. **Connection Class**: `aws-sns-connection` → `aws2-sns-connection`
3. **Producer Class**: `aws-sns-producer` → `aws2-sns-producer`
4. **Credentials**: Use `aws2-*-credentials-builder` classes
5. **Endpoint**: `endpoint-override` instead of `custom-endpoint`

## Additional Resources

- [AWS SNS Documentation](https://docs.aws.amazon.com/sns/latest/dg/welcome.html)
- [AWS SDK for Java 2.x](https://docs.aws.amazon.com/sdk-for-java/latest/developer-guide/home.html)
- [Interlok AWS SNS (SDK v1)](../interlok-aws-sns/)
- [Interlok Documentation](https://interlok.adaptris.net/)

## License

This component is licensed under the Apache License 2.0.
