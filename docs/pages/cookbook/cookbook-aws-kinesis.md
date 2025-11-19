# Interlok AWS Kinesis

Interlok AWS Kinesis provides integration with Amazon Kinesis Data Streams using the Kinesis Producer Library (KPL) for high-performance, reliable data ingestion.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Architecture](#architecture)
- [Connection Types](#connection-types)
    - [Connection from Properties](#connection-from-properties)
    - [Inline Producer Configuration](#inline-producer-configuration)
- [Producers](#producers)
    - [Kinesis Stream Producer](#kinesis-stream-producer)
    - [Kinesis Synchronous Stream Producer](#kinesis-synchronous-stream-producer)
- [Configuration](#configuration)
- [Examples](#examples)
- [Best Practices](#best-practices)
- [Troubleshooting](#troubleshooting)

## Overview

The `interlok-aws-kinesis` component provides producer functionality for Amazon Kinesis Data Streams using the **Kinesis Producer Library (KPL)**. This library offers:

- **High Performance**: Batching and aggregation for optimal throughput
- **Reliability**: Automatic retries and error handling
- **Monitoring**: Built-in CloudWatch metrics
- **Asynchronous Processing**: Non-blocking operations for better performance

**Key Features:**
- Produce messages to Kinesis streams
- Configurable partition keys for data distribution
- Asynchronous and synchronous producer modes
- Flexible connection configuration via properties or inline
- Support for custom AWS credentials providers

**Use Cases:**
- Real-time data streaming
- Log aggregation
- Event processing pipelines
- IoT data ingestion
- Clickstream analytics

## Installation

Add the following dependency to your Interlok installation:

```xml
<dependency>
    <groupId>com.adaptris</groupId>
    <artifactId>interlok-aws-kinesis</artifactId>
    <version>4.x.x</version>
</dependency>
```

## Architecture

The Kinesis Producer Library (KPL) provides several advantages:

1. **Batching**: Automatically batches multiple records into a single request
2. **Aggregation**: Combines multiple user records into a single Kinesis record
3. **Retries**: Automatic retry logic with exponential backoff
4. **Monitoring**: Publishes metrics to CloudWatch
5. **Asynchronous**: Non-blocking API for high throughput

## Connection Types

### Connection from Properties

Load KPL configuration from a properties file.

**Class:** `aws-kinesis-kpl-connection-from-properties`

**Configuration:**

```xml
<connection class="aws-kinesis-kpl-connection-from-properties">
    <unique-id>kinesis-connection</unique-id>
    <config-location>file:///path/to/kinesis-config.properties</config-location>
</connection>
```

**Properties:**

| Property | Description | Required |
|----------|-------------|----------|
| `config-location` | URL to properties file containing KPL configuration | Yes |

**Notes:**
- Uses `DefaultAWSCredentialsProviderChain` for authentication
- Cannot override credentials provider via properties file
- Properties file format follows [KPL configuration](https://github.com/awslabs/amazon-kinesis-producer/blob/master/java/amazon-kinesis-producer-sample/default_config.properties)

**Sample Properties File:**

```properties
# AWS Region
Region=us-east-1

# Kinesis endpoint (optional, for custom endpoints)
# KinesisEndpoint=kinesis.us-east-1.amazonaws.com
# KinesisPort=443

# Aggregation settings
AggregationEnabled=true
AggregationMaxCount=4294967295
AggregationMaxSize=51200

# Collection settings
CollectionMaxCount=500
CollectionMaxSize=5242880

# Retry settings
RecordMaxBufferedTime=100
RecordTtl=30000
MaxConnections=24

# Metrics
MetricsLevel=detailed
MetricsGranularity=shard
MetricsNamespace=KinesisProducerLibrary

# CloudWatch endpoint (optional)
# CloudwatchEndpoint=monitoring.us-east-1.amazonaws.com
# CloudwatchPort=443
```

### Inline Producer Configuration

Configure KPL settings inline with custom credentials support.

**Class:** `aws-kinesis-kpl-inline-connection`

**Configuration:**

```xml
<connection class="aws-kinesis-kpl-inline-connection">
    <unique-id>kinesis-connection</unique-id>
    <credentials class="aws-static-credentials-builder">
        <access-key>YOUR_ACCESS_KEY</access-key>
        <secret-key>YOUR_SECRET_KEY</secret-key>
    </credentials>
    <config>
        <key-value-pair>
            <key>Region</key>
            <value>us-east-1</value>
        </key-value-pair>
        <key-value-pair>
            <key>AggregationEnabled</key>
            <value>true</value>
        </key-value-pair>
        <key-value-pair>
            <key>RecordMaxBufferedTime</key>
            <value>100</value>
        </key-value-pair>
    </config>
</connection>
```

**Properties:**

| Property | Description | Required | Default |
|----------|-------------|----------|---------|
| `credentials` | AWS credentials provider for Kinesis | No | DefaultAWSCredentialsProviderChain |
| `metrics-credentials` | Separate credentials for CloudWatch metrics | No | Same as credentials |
| `config` | Key-value pairs for KPL configuration | No | Empty |

**Available Configuration Keys:**

| Key | Description | Default |
|-----|-------------|---------|
| `Region` | AWS region | - |
| `AggregationEnabled` | Enable record aggregation | true |
| `AggregationMaxCount` | Max records per aggregate | 4294967295 |
| `AggregationMaxSize` | Max size of aggregate in bytes | 51200 |
| `CollectionMaxCount` | Max records per request | 500 |
| `CollectionMaxSize` | Max size of request in bytes | 5242880 |
| `RecordMaxBufferedTime` | Max time to buffer records (ms) | 100 |
| `RecordTtl` | Time to live for records (ms) | 30000 |
| `MaxConnections` | Max HTTP connections | 24 |
| `MetricsLevel` | CloudWatch metrics level (none/summary/detailed) | detailed |
| `MetricsGranularity` | Metrics granularity (global/stream/shard) | shard |
| `MetricsNamespace` | CloudWatch namespace | KinesisProducerLibrary |

## Producers

### Kinesis Stream Producer

Asynchronous producer that sends records to Kinesis without waiting for confirmation.

**Class:** `aws-kinesis-stream-producer`

**Configuration:**

```xml
<producer class="aws-kinesis-stream-producer">
    <stream>my-kinesis-stream</stream>
    <partition-key>%message{partitionKey}</partition-key>
</producer>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `stream` | Kinesis stream name | Yes | Yes |
| `partition-key` | Partition key for record distribution | Yes | Yes |

**Behavior:**
- Records are sent asynchronously
- Does not wait for confirmation from Kinesis
- Higher throughput due to non-blocking operation
- Suitable for high-volume scenarios where occasional loss is acceptable

### Kinesis Synchronous Stream Producer

Synchronous producer that waits for confirmation before completing.

**Class:** `aws-kinesis-synchronous-stream-producer`

**Configuration:**

```xml
<producer class="aws-kinesis-synchronous-stream-producer">
    <stream>my-kinesis-stream</stream>
    <partition-key>%message{customerId}</partition-key>
</producer>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `stream` | Kinesis stream name | Yes | Yes |
| `partition-key` | Partition key for record distribution | Yes | Yes |

**Behavior:**
- Waits for Kinesis to confirm record receipt
- Logs the result (shard ID, sequence number)
- Lower throughput but guaranteed delivery confirmation
- Suitable for critical data where confirmation is required

**Result Logging:**
The synchronous producer logs detailed information about each record:
- Shard ID where the record was stored
- Sequence number assigned by Kinesis
- Success/failure status

## Configuration

### Partition Keys

Partition keys determine how records are distributed across shards:

**Static Partition Key:**
```xml
<partition-key>fixed-key</partition-key>
```

**Dynamic Partition Key from Metadata:**
```xml
<partition-key>%message{userId}</partition-key>
```

**Dynamic Partition Key from Payload:**
```xml
<partition-key>%message{jsonPath:$.customerId}</partition-key>
```

**Best Practices for Partition Keys:**
- Use high-cardinality keys for even distribution
- Avoid hot partitions by distributing load evenly
- Consider using customer ID, user ID, or device ID
- Avoid timestamp-based keys that create hot spots

### Stream Names

Stream names can be static or dynamic:

**Static Stream:**
```xml
<stream>production-events</stream>
```

**Dynamic Stream from Metadata:**
```xml
<stream>%message{streamName}</stream>
```

**Dynamic Stream with Prefix:**
```xml
<stream>events-%message{environment}</stream>
```

## Examples

### Example 1: Basic Kinesis Producer with Properties File

```xml
<channel>
    <consume-connection class="null-connection"/>
    <produce-connection class="aws-kinesis-kpl-connection-from-properties">
        <unique-id>kinesis-conn</unique-id>
        <config-location>file:///opt/interlok/config/kinesis.properties</config-location>
    </produce-connection>

    <workflow>
        <consumer class="..."/>
        <service-collection class="service-list"/>
        <producer class="aws-kinesis-stream-producer">
            <stream>application-events</stream>
            <partition-key>%message{eventId}</partition-key>
        </producer>
    </workflow>
</channel>
```

### Example 2: Inline Configuration with Custom Credentials

```xml
<channel>
    <consume-connection class="null-connection"/>
    <produce-connection class="aws-kinesis-kpl-inline-connection">
        <unique-id>kinesis-conn</unique-id>
        <credentials class="aws-static-credentials-builder">
            <access-key>${aws.access.key}</access-key>
            <secret-key>${aws.secret.key}</secret-key>
        </credentials>
        <config>
            <key-value-pair>
                <key>Region</key>
                <value>us-east-1</value>
            </key-value-pair>
            <key-value-pair>
                <key>AggregationEnabled</key>
                <value>true</value>
            </key-value-pair>
            <key-value-pair>
                <key>RecordMaxBufferedTime</key>
                <value>100</value>
            </key-value-pair>
            <key-value-pair>
                <key>MetricsLevel</key>
                <value>detailed</value>
            </key-value-pair>
        </config>
    </produce-connection>

    <workflow>
        <consumer class="..."/>
        <service-collection class="service-list"/>
        <producer class="aws-kinesis-stream-producer">
            <stream>user-activity</stream>
            <partition-key>%message{userId}</partition-key>
        </producer>
    </workflow>
</channel>
```

### Example 3: Synchronous Producer for Critical Data

```xml
<channel>
    <consume-connection class="null-connection"/>
    <produce-connection class="aws-kinesis-kpl-inline-connection">
        <unique-id>kinesis-conn</unique-id>
        <credentials class="aws-default-credentials-provider"/>
        <config>
            <key-value-pair>
                <key>Region</key>
                <value>eu-west-1</value>
            </key-value-pair>
        </config>
    </produce-connection>

    <workflow>
        <consumer class="..."/>
        <service-collection class="service-list"/>
        <producer class="aws-kinesis-synchronous-stream-producer">
            <stream>financial-transactions</stream>
            <partition-key>%message{transactionId}</partition-key>
        </producer>
    </workflow>
</channel>
```

### Example 4: Multi-Stream Routing

```xml
<channel>
    <consume-connection class="null-connection"/>
    <produce-connection class="aws-kinesis-kpl-inline-connection">
        <unique-id>kinesis-conn</unique-id>
        <credentials class="aws-default-credentials-provider"/>
        <config>
            <key-value-pair>
                <key>Region</key>
                <value>us-west-2</value>
            </key-value-pair>
        </config>
    </produce-connection>

    <workflow>
        <consumer class="..."/>
        <service-collection class="service-list">
            <services>
                <!-- Set stream name based on message type -->
                <add-metadata-service>
                    <metadata-element>
                        <key>streamName</key>
                        <value>%message{jsonPath:$.eventType}-events</value>
                    </metadata-element>
                </add-metadata-service>
            </services>
        </service-collection>
        <producer class="aws-kinesis-stream-producer">
            <stream>%message{streamName}</stream>
            <partition-key>%message{jsonPath:$.id}</partition-key>
        </producer>
    </workflow>
</channel>
```

### Example 5: High-Throughput Configuration

```xml
<produce-connection class="aws-kinesis-kpl-inline-connection">
    <unique-id>high-throughput-kinesis</unique-id>
    <credentials class="aws-default-credentials-provider"/>
    <config>
        <key-value-pair>
            <key>Region</key>
            <value>us-east-1</value>
        </key-value-pair>
        <!-- Enable aggregation for better throughput -->
        <key-value-pair>
            <key>AggregationEnabled</key>
            <value>true</value>
        </key-value-pair>
        <!-- Increase buffer time for better batching -->
        <key-value-pair>
            <key>RecordMaxBufferedTime</key>
            <value>500</value>
        </key-value-pair>
        <!-- Increase max connections -->
        <key-value-pair>
            <key>MaxConnections</key>
            <value>48</value>
        </key-value-pair>
        <!-- Larger collection sizes -->
        <key-value-pair>
            <key>CollectionMaxCount</key>
            <value>1000</value>
        </key-value-pair>
    </config>
</produce-connection>
```

### Example 6: Custom Endpoint (LocalStack/Testing)

```xml
<produce-connection class="aws-kinesis-kpl-inline-connection">
    <unique-id>localstack-kinesis</unique-id>
    <credentials class="aws-static-credentials-builder">
        <access-key>test</access-key>
        <secret-key>test</secret-key>
    </credentials>
    <config>
        <key-value-pair>
            <key>Region</key>
            <value>us-east-1</value>
        </key-value-pair>
        <key-value-pair>
            <key>KinesisEndpoint</key>
            <value>localhost</value>
        </key-value-pair>
        <key-value-pair>
            <key>KinesisPort</key>
            <value>4566</value>
        </key-value-pair>
        <key-value-pair>
            <key>CloudwatchEndpoint</key>
            <value>localhost</value>
        </key-value-pair>
        <key-value-pair>
            <key>CloudwatchPort</key>
            <value>4566</value>
        </key-value-pair>
        <key-value-pair>
            <key>VerifyCertificate</key>
            <value>false</value>
        </key-value-pair>
    </config>
</produce-connection>
```

## Best Practices

### 1. Partition Key Selection

**Do:**
- Use high-cardinality keys (user ID, device ID, transaction ID)
- Distribute load evenly across shards
- Use consistent hashing for related records

**Don't:**
- Use timestamp-based keys (creates hot partitions)
- Use low-cardinality keys (limits parallelism)
- Use sequential keys (uneven distribution)

### 2. Performance Optimization

**Enable Aggregation:**
```xml
<key-value-pair>
    <key>AggregationEnabled</key>
    <value>true</value>
</key-value-pair>
```

**Tune Buffer Time:**
- Lower values (50-100ms): Lower latency, less batching
- Higher values (500-1000ms): Better throughput, higher latency

**Adjust Connection Pool:**
```xml
<key-value-pair>
    <key>MaxConnections</key>
    <value>48</value>
</key-value-pair>
```

### 3. Error Handling

**Use Synchronous Producer for Critical Data:**
- Financial transactions
- Audit logs
- Critical events

**Use Asynchronous Producer for High Volume:**
- Clickstream data
- Application logs
- Metrics

### 4. Monitoring

**Enable Detailed Metrics:**
```xml
<key-value-pair>
    <key>MetricsLevel</key>
    <value>detailed</value>
</key-value-pair>
<key-value-pair>
<key>MetricsGranularity</key>
<value>shard</value>
</key-value-pair>
```

**Monitor Key Metrics:**
- `UserRecordsPut`: Number of records sent
- `UserRecordsDataPut`: Bytes sent
- `KinesisRecordsPut`: Actual Kinesis API calls
- `ErrorsByCode`: Error rates by type
- `UserRecordExpired`: Records that expired before sending

### 5. Resource Management

**Set Appropriate TTL:**
```xml
<key-value-pair>
    <key>RecordTtl</key>
    <value>30000</value>
</key-value-pair>
```

**Configure Request Timeout:**
```xml
<key-value-pair>
    <key>RequestTimeout</key>
    <value>6000</value>
</key-value-pair>
```

### 6. Credentials Management

**Use IAM Roles (Recommended):**
```xml
<credentials class="aws-default-credentials-provider"/>
```

**Use Separate Metrics Credentials (Optional):**
```xml
<metrics-credentials class="aws-static-credentials-builder">
    <access-key>${metrics.access.key}</access-key>
    <secret-key>${metrics.secret.key}</secret-key>
</metrics-credentials>
```

### 7. Stream Capacity Planning

**Calculate Required Shards:**
- Each shard: 1 MB/s or 1000 records/s
- Monitor `WriteProvisionedThroughputExceeded` metric
- Scale shards based on traffic patterns

### 8. Data Retention

**Configure Stream Retention:**
- Default: 24 hours
- Extended: Up to 365 days
- Plan consumer processing accordingly

## Troubleshooting

### Connection Issues

**Problem:** Cannot connect to Kinesis

**Solutions:**
- Verify AWS credentials are correct
- Check region configuration
- Ensure network connectivity to Kinesis endpoints
- Verify IAM permissions for `kinesis:PutRecord` and `kinesis:PutRecords`

**Problem:** Connection timeout

**Solutions:**
- Increase `RequestTimeout` configuration
- Check network latency
- Verify firewall rules allow HTTPS traffic

### Performance Issues

**Problem:** Low throughput

**Solutions:**
- Enable aggregation: `AggregationEnabled=true`
- Increase buffer time: `RecordMaxBufferedTime=500`
- Increase max connections: `MaxConnections=48`
- Check shard capacity and scale if needed

**Problem:** High latency

**Solutions:**
- Reduce buffer time: `RecordMaxBufferedTime=50`
- Use synchronous producer for immediate confirmation
- Check CloudWatch metrics for bottlenecks

### Data Loss Issues

**Problem:** Records not appearing in stream

**Solutions:**
- Use synchronous producer to verify delivery
- Check CloudWatch metrics for errors
- Verify stream exists and is active
- Check `UserRecordExpired` metric for TTL issues

**Problem:** Records expiring before delivery

**Solutions:**
- Increase TTL: `RecordTtl=60000`
- Reduce buffer time for faster delivery
- Check for network issues causing delays

### Error Handling

**Problem:** `ProvisionedThroughputExceededException`

**Solutions:**
- Increase shard count
- Improve partition key distribution
- Enable aggregation for better batching
- Implement exponential backoff (KPL handles this automatically)

**Problem:** `InvalidArgumentException`

**Solutions:**
- Verify partition key is not empty
- Check record size (max 1 MB)
- Ensure stream name is valid

### Platform-Specific Issues

**Problem:** Native binary errors on Windows

**Solutions:**
- Verify KPL version includes Windows binaries
- Check [KPL compatibility](https://github.com/awslabs/amazon-kinesis-producer)
- Consider using specific KPL version with Windows support

**Problem:** Native binary errors on Alpine Linux/Docker

**Solutions:**
- Use glibc-based Docker images instead of Alpine (musl-based)
- Example: Use `openjdk:11` instead of `openjdk:11-alpine`
- Or install glibc compatibility layer in Alpine

### Monitoring and Debugging

**Enable Debug Logging:**
```xml
<key-value-pair>
    <key>LogLevel</key>
    <value>debug</value>
</key-value-pair>
```

**Check CloudWatch Metrics:**
- Navigate to CloudWatch → Metrics → KinesisProducerLibrary
- Monitor error rates, throughput, and latency
- Set up alarms for critical metrics

**Review Application Logs:**
- Synchronous producer logs shard ID and sequence number
- Check for exception stack traces
- Monitor for retry attempts

## Platform Compatibility

### Operating Systems

| OS | Support | Notes |
|----|---------|-------|
| Linux (glibc) | ✅ Full | Recommended for production |
| macOS | ✅ Full | Supported for development |
| Windows | ⚠️ Limited | Check KPL version for Windows binaries |
| Alpine Linux | ❌ Not Supported | Use glibc-based images |

### Docker Considerations

**Recommended Base Images:**
- `openjdk:11`
- `amazoncorretto:11`
- `eclipse-temurin:11`

**Avoid:**
- Alpine-based images (musl libc incompatibility)

**Example Dockerfile:**
```dockerfile
FROM openjdk:11-jre-slim
COPY interlok /opt/interlok
WORKDIR /opt/interlok
CMD ["java", "-jar", "lib/interlok-boot.jar"]
```

## KPL Configuration Reference

### Complete Configuration Example

```properties
# Required
Region=us-east-1

# Endpoints (optional, for custom/testing)
KinesisEndpoint=kinesis.us-east-1.amazonaws.com
KinesisPort=443
CloudwatchEndpoint=monitoring.us-east-1.amazonaws.com
CloudwatchPort=443

# Aggregation
AggregationEnabled=true
AggregationMaxCount=4294967295
AggregationMaxSize=51200

# Collection
CollectionMaxCount=500
CollectionMaxSize=5242880

# Buffering
RecordMaxBufferedTime=100
RecordTtl=30000

# Connections
MaxConnections=24
RequestTimeout=6000
ConnectTimeout=6000

# Retries
RateLimit=150

# Metrics
MetricsLevel=detailed
MetricsGranularity=shard
MetricsNamespace=KinesisProducerLibrary
MetricsUploadDelay=60000

# Logging
LogLevel=info

# Security
VerifyCertificate=true
```

## Additional Resources

- [AWS Kinesis Data Streams Documentation](https://docs.aws.amazon.com/kinesis/latest/dev/introduction.html)
- [Kinesis Producer Library (KPL)](https://docs.aws.amazon.com/streams/latest/dev/developing-producers-with-kpl.html)
- [KPL GitHub Repository](https://github.com/awslabs/amazon-kinesis-producer)
- [Interlok Documentation](https://interlok.adaptris.net/)
- [AWS SDK for Java](https://aws.amazon.com/sdk-for-java/)

## License

This component is licensed under the Apache License 2.0.
