# Interlok AWS KMS (SDK v2)

Interlok AWS KMS provides integration with AWS Key Management Service (KMS) for encryption, decryption, and digital signature operations using customer-managed keys. This version uses **AWS SDK v2**.

> **Note:** This is the AWS SDK v2 implementation. For the SDK v1 version, see [interlok-aws-kms](../interlok-aws-kms/).

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [SDK v2 vs SDK v1](#sdk-v2-vs-sdk-v1)
- [Connection Configuration](#connection-configuration)
- [Services](#services)
- [Configuration](#configuration)
- [Examples](#examples)
- [Best Practices](#best-practices)
- [Troubleshooting](#troubleshooting)

## Overview

The `interlok-aws2-kms` component provides services for cryptographic operations using AWS Key Management Service (KMS) with AWS SDK v2. KMS is a managed service that makes it easy to create and control encryption keys used to encrypt your data.

**Key Features:**
- Encrypt and decrypt data using KMS customer master keys (CMKs)
- Generate and verify digital signatures
- Support for encryption context for additional security
- Multiple encryption and signing algorithms
- Integration with AWS IAM for access control
- Built on AWS SDK v2 for improved performance and features

**Use Cases:**
- Encrypt sensitive data before storage
- Decrypt encrypted data for processing
- Sign data for integrity verification
- Verify signatures to ensure data authenticity
- Secure API communications
- Compliance with data protection regulations

## Installation

Add the following dependency to your Interlok installation:

```xml
<dependency>
  <groupId>com.adaptris</groupId>
  <artifactId>interlok-aws2-kms</artifactId>
  <version>4.x.x</version>
</dependency>
```

## SDK v2 vs SDK v1

### Why Use SDK v2?

**Advantages of AWS SDK v2:**
- **Better Performance**: Improved HTTP client with connection pooling
- **Non-blocking I/O**: Asynchronous operations support
- **Smaller Footprint**: Reduced dependency size
- **Modern API**: Cleaner, more intuitive API design
- **Active Development**: AWS focuses development on SDK v2
- **Better Resource Management**: Improved connection and memory management

### Migration from SDK v1

The configuration and usage are nearly identical between SDK v1 and v2 versions. The main differences are:

1. **Artifact Name**: `interlok-aws-kms` → `interlok-aws2-kms`
2. **Connection Class**: Uses AWS SDK v2 internally
3. **Dependencies**: Different underlying AWS SDK libraries

**Configuration remains the same**, making migration straightforward.

## Connection Configuration

### Basic Connection

```xml
<connection class="aws2-kms-connection">
  <unique-id>kms-connection</unique-id>
  <region>us-east-1</region>
  <credentials class="aws2-static-credentials-builder">
    <access-key>YOUR_ACCESS_KEY</access-key>
    <secret-key>YOUR_SECRET_KEY</secret-key>
  </credentials>
</connection>
```

### Connection with Custom Endpoint

For use with LocalStack or custom KMS endpoints:

```xml
<connection class="aws2-kms-connection">
  <unique-id>localstack-kms</unique-id>
  <region>us-east-1</region>
  <credentials class="aws2-static-credentials-builder">
    <access-key>test</access-key>
    <secret-key>test</secret-key>
  </credentials>
  <endpoint-override>http://localhost:4566</endpoint-override>
</connection>
```

### Connection Properties

| Property | Description | Required | Default |
|----------|-------------|----------|---------|
| `region` | AWS region where KMS keys are located | Yes | - |
| `credentials` | AWS credentials provider (SDK v2) | Yes | - |
| `endpoint-override` | Custom KMS endpoint URL | No | AWS KMS |
| `client-override-configuration` | Advanced client configuration | No | - |
| `retry-policy` | Custom retry policy | No | - |

## Services

### Encrypt Service

Encrypt data using an AWS KMS customer master key (CMK).

**Class:** `aws2-kms-encrypt-data`

**Configuration:**

```xml
<service class="aws2-kms-encrypt-data">
  <connection class="aws2-kms-connection">
    <!-- connection config -->
  </connection>
  <key-id>arn:aws:kms:us-east-1:123456789012:key/12345678-1234-1234-1234-123456789012</key-id>
  <input class="payload-stream-input-parameter"/>
  <output class="payload-stream-output-parameter"/>
  <encryption-algorithm>SYMMETRIC_DEFAULT</encryption-algorithm>
  <encryption-context>
    <key-value-pair>
      <key>Department</key>
      <value>Finance</value>
    </key-value-pair>
  </encryption-context>
</service>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `key-id` | KMS key ID, ARN, or alias | Yes | Yes |
| `input` | Source of data to encrypt | No | PayloadStreamInputParameter |
| `output` | Destination for encrypted data | No | PayloadStreamOutputParameter |
| `encryption-algorithm` | Encryption algorithm to use | No | SYMMETRIC_DEFAULT |
| `encryption-context` | Additional authenticated data | No | Empty |

**Encryption Algorithms:**
- `SYMMETRIC_DEFAULT` (AES-GCM with 256-bit key)
- `RSAES_OAEP_SHA_1`
- `RSAES_OAEP_SHA_256`

**Notes:**
- Maximum plaintext size: 4 KB for direct encryption
- For larger data, use envelope encryption pattern
- Encryption context provides additional security and audit trail

### Decrypt Service

Decrypt data that was encrypted using AWS KMS.

**Class:** `aws2-kms-decrypt-data`

**Configuration:**

```xml
<service class="aws2-kms-decrypt-data">
  <connection class="aws2-kms-connection">
    <!-- connection config -->
  </connection>
  <key-id>arn:aws:kms:us-east-1:123456789012:key/12345678-1234-1234-1234-123456789012</key-id>
  <input class="payload-stream-input-parameter"/>
  <output class="payload-stream-output-parameter"/>
  <encryption-algorithm>SYMMETRIC_DEFAULT</encryption-algorithm>
  <encryption-context>
    <key-value-pair>
      <key>Department</key>
      <value>Finance</value>
    </key-value-pair>
  </encryption-context>
</service>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `key-id` | KMS key ID, ARN, or alias | Yes | Yes |
| `input` | Source of encrypted data | No | PayloadStreamInputParameter |
| `output` | Destination for decrypted data | No | PayloadStreamOutputParameter |
| `encryption-algorithm` | Encryption algorithm used | No | SYMMETRIC_DEFAULT |
| `encryption-context` | Must match encryption context used during encryption | No | Empty |

**Notes:**
- Encryption context must match exactly what was used during encryption
- KMS automatically determines which key was used for encryption
- `key-id` parameter is optional but recommended for performance

### Generate Signature Service

Generate a digital signature using an asymmetric KMS key.

**Class:** `aws2-kms-generate-signature`

**Configuration:**

```xml
<service class="aws2-kms-generate-signature">
  <connection class="aws2-kms-connection">
    <!-- connection config -->
  </connection>
  <key-id>arn:aws:kms:us-east-1:123456789012:key/12345678-1234-1234-1234-123456789012</key-id>
  <signing-algorithm>RSASSA_PSS_SHA_256</signing-algorithm>
  <message-type>DIGEST</message-type>
  <input class="byte-array-from-metadata">
    <metadata-key>dataHash</metadata-key>
  </input>
  <output class="metadata-stream-output">
    <metadata-key>signature</metadata-key>
  </output>
</service>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `key-id` | KMS asymmetric key ID or ARN | Yes | Yes |
| `signing-algorithm` | Algorithm for signing | Yes | Yes |
| `message-type` | Type of data being signed | No | RAW |
| `input` | Source of data to sign (max 4096 bytes) | Yes | - |
| `output` | Destination for signature | Yes | - |

**Signing Algorithms:**
- `RSASSA_PSS_SHA_256`
- `RSASSA_PSS_SHA_384`
- `RSASSA_PSS_SHA_512`
- `RSASSA_PKCS1_V1_5_SHA_256`
- `RSASSA_PKCS1_V1_5_SHA_384`
- `RSASSA_PKCS1_V1_5_SHA_512`
- `ECDSA_SHA_256`
- `ECDSA_SHA_384`
- `ECDSA_SHA_512`

**Message Types:**
- `RAW`: Sign the raw message (max 4096 bytes)
- `DIGEST`: Sign a pre-computed hash

### Verify Signature Service

Verify a digital signature using an asymmetric KMS key.

**Class:** `aws2-kms-verify-signature`

**Configuration:**

```xml
<service class="aws2-kms-verify-signature">
  <connection class="aws2-kms-connection">
    <!-- connection config -->
  </connection>
  <key-id>arn:aws:kms:us-east-1:123456789012:key/12345678-1234-1234-1234-123456789012</key-id>
  <signing-algorithm>RSASSA_PSS_SHA_256</signing-algorithm>
  <message-type>DIGEST</message-type>
  <data-to-be-verified class="byte-array-from-metadata">
    <metadata-key>dataHash</metadata-key>
  </data-to-be-verified>
  <signature class="byte-array-from-metadata">
    <metadata-key>signature</metadata-key>
  </signature>
</service>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `key-id` | KMS asymmetric key ID or ARN | Yes | Yes |
| `signing-algorithm` | Algorithm used for signing | Yes | Yes |
| `message-type` | Type of data being verified | No | RAW |
| `data-to-be-verified` | Original data or hash | Yes | - |
| `signature` | Signature to verify | Yes | - |

## Configuration

For detailed configuration options including:
- Key identifiers (ID, ARN, alias formats)
- Input/Output wrappers
- Encryption context
- IAM permissions
- Key types and specifications

Please refer to the [interlok-aws-kms documentation](../interlok-aws-kms/README.md), as the configuration is identical between SDK v1 and v2 versions.

## Examples

### Example 1: Basic Encryption and Decryption

```xml
<service-list>
  <services>
    <!-- Encrypt payload -->
    <service class="aws2-kms-encrypt-data">
      <connection class="aws2-kms-connection">
        <unique-id>kms-conn</unique-id>
        <region>us-east-1</region>
        <credentials class="aws2-default-credentials-provider"/>
      </connection>
      <key-id>alias/my-encryption-key</key-id>
      <input class="payload-stream-input-parameter"/>
      <output class="payload-stream-output-parameter"/>
    </service>
    
    <!-- Later: Decrypt payload -->
    <service class="aws2-kms-decrypt-data">
      <connection class="aws2-kms-connection">
        <unique-id>kms-conn</unique-id>
        <region>us-east-1</region>
        <credentials class="aws2-default-credentials-provider"/>
      </connection>
      <key-id>alias/my-encryption-key</key-id>
      <input class="payload-stream-input-parameter"/>
      <output class="payload-stream-output-parameter"/>
    </service>
  </services>
</service-list>
```

### Example 2: Sign and Verify with SDK v2

```xml
<service-list>
  <services>
    <!-- Generate hash -->
    <generate-digest-service>
      <algorithm>SHA-256</algorithm>
      <metadata-key>payloadHash</metadata-key>
    </generate-digest-service>
    
    <!-- Sign the hash -->
    <service class="aws2-kms-generate-signature">
      <connection class="aws2-kms-connection">
        <unique-id>kms-conn</unique-id>
        <region>us-east-1</region>
        <credentials class="aws2-default-credentials-provider"/>
      </connection>
      <key-id>alias/my-signing-key</key-id>
      <signing-algorithm>RSASSA_PSS_SHA_256</signing-algorithm>
      <message-type>DIGEST</message-type>
      <input class="byte-array-from-metadata">
        <metadata-key>payloadHash</metadata-key>
      </input>
      <output class="metadata-stream-output">
        <metadata-key>signature</metadata-key>
        <content-encoding>base64</content-encoding>
      </output>
    </service>
    
    <!-- Verify the signature -->
    <service class="aws2-kms-verify-signature">
      <connection class="aws2-kms-connection">
        <unique-id>kms-conn</unique-id>
        <region>us-east-1</region>
        <credentials class="aws2-default-credentials-provider"/>
      </connection>
      <key-id>alias/my-signing-key</key-id>
      <signing-algorithm>RSASSA_PSS_SHA_256</signing-algorithm>
      <message-type>DIGEST</message-type>
      <data-to-be-verified class="byte-array-from-metadata">
        <metadata-key>payloadHash</metadata-key>
      </data-to-be-verified>
      <signature class="byte-array-from-metadata">
        <metadata-key>signature</metadata-key>
        <content-encoding>base64</content-encoding>
      </signature>
    </service>
  </services>
</service-list>
```

### Example 3: LocalStack Testing with SDK v2

```xml
<connection class="aws2-kms-connection">
  <unique-id>localstack-kms</unique-id>
  <region>us-east-1</region>
  <credentials class="aws2-static-credentials-builder">
    <access-key>test</access-key>
    <secret-key>test</secret-key>
  </credentials>
  <endpoint-override>http://localhost:4566</endpoint-override>
</connection>
```

For more examples including:
- Encryption with context
- Envelope encryption pattern
- Multi-region keys
- Dynamic key selection
- Error handling

Please refer to the [interlok-aws-kms examples](../interlok-aws-kms/README.md#examples).

## Best Practices

### SDK v2 Specific

**Use Default Credentials Provider:**
```xml
<credentials class="aws2-default-credentials-provider"/>
```
- Automatically uses IAM roles, environment variables, or credentials file
- More secure than hardcoded credentials
- Follows AWS best practices

**Connection Pooling:**
- SDK v2 automatically manages connection pooling
- Better resource utilization than SDK v1
- No additional configuration needed

For comprehensive best practices including:
- Key management strategies
- Encryption context usage
- Performance optimization
- Security practices
- Cost optimization
- Compliance and auditing

Please refer to the [interlok-aws-kms best practices](../interlok-aws-kms/README.md#best-practices).

## Troubleshooting

### SDK v2 Specific Issues

**Problem:** Dependency conflicts with SDK v1

**Solution:**
- Ensure only one SDK version is in classpath
- Use `interlok-aws2-*` artifacts consistently
- Check for transitive dependencies

**Problem:** Different error messages than SDK v1

**Solution:**
- SDK v2 may have different exception types
- Update error handling if migrating from SDK v1
- Consult AWS SDK v2 documentation for exception hierarchy

For comprehensive troubleshooting including:
- Connection issues
- Encryption/decryption problems
- Signature verification
- Performance issues
- Common error messages

Please refer to the [interlok-aws-kms troubleshooting](../interlok-aws-kms/README.md#troubleshooting).

## Additional Resources

- [AWS KMS Documentation](https://docs.aws.amazon.com/kms/latest/developerguide/overview.html)
- [AWS SDK for Java 2.x](https://docs.aws.amazon.com/sdk-for-java/latest/developer-guide/home.html)
- [AWS SDK v2 Migration Guide](https://docs.aws.amazon.com/sdk-for-java/latest/migration-guide/what-is-java-migration.html)
- [Interlok AWS KMS (SDK v1)](../interlok-aws-kms/README.md)
- [Interlok Documentation](https://interlok.adaptris.net/)

## License

This component is licensed under the Apache License 2.0.
