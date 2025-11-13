# Interlok AWS2 S3

Interlok AWS2 S3 provides comprehensive integration with Amazon S3 (Simple Storage Service) using AWS SDK v2 for uploading, downloading, copying, deleting, and managing objects in S3 buckets.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Migration from AWS SDK v1](#migration-from-aws-sdk-v1)
- [Connection Configuration](#connection-configuration)
- [Operations](#operations)
    - [Upload Operation](#upload-operation)
    - [Download Operation](#download-operation)
    - [Copy Operation](#copy-operation)
    - [Extended Copy Operation](#extended-copy-operation)
    - [Delete Operation](#delete-operation)
    - [List Operation](#list-operation)
    - [Check File Exists Operation](#check-file-exists-operation)
    - [Tag Operation](#tag-operation)
    - [Get Tag Operation](#get-tag-operation)
- [Object Metadata](#object-metadata)
- [Access Control Lists (ACL)](#access-control-lists-acl)
- [Retry Store](#retry-store)
- [Examples](#examples)

## Overview

The `interlok-aws2-s3` component provides a service-based approach to interact with Amazon S3 using **AWS SDK v2**. This is the modern, recommended version for new implementations.

**Key Features:**
- Uploading and downloading objects
- Copying objects within S3
- Deleting objects
- Listing objects with filtering
- Managing object metadata and tags
- Setting access control lists (ACLs)
- Using S3 as a retry/failed message store
- Built on AWS SDK v2 for improved performance and features

**Why AWS SDK v2?**
- Better performance and reduced memory footprint
- Non-blocking I/O support
- Improved pagination
- Better exception handling
- Active development and support from AWS

## Installation

Add the following dependency to your Interlok installation:

```xml
<dependency>
  <groupId>com.adaptris</groupId>
  <artifactId>interlok-aws2-s3</artifactId>
  <version>4.x.x</version>
</dependency>
```

## Migration from AWS SDK v1

If you're migrating from `interlok-aws-s3` (AWS SDK v1) to `interlok-aws2-s3` (AWS SDK v2), the main changes are:

### Connection Class Name
- **v1:** `amazon-s3-connection`
- **v2:** `aws2-amazon-s3-connection`

### Service Class Name
- **v1:** `amazon-s3-service`
- **v2:** `aws2-amazon-s3-service`

### Operation Class Names
All operation classes are prefixed with `aws2-`:
- **v1:** `amazon-s3-upload` → **v2:** `aws2-amazon-s3-upload`
- **v1:** `amazon-s3-download` → **v2:** `aws2-amazon-s3-download`
- **v1:** `amazon-s3-copy` → **v2:** `aws2-amazon-s3-copy`
- And so on...

### Configuration Compatibility
Most configuration properties remain the same, making migration straightforward. The XML structure and operation parameters are largely compatible.

## Connection Configuration

### Basic Connection

```xml
<connection class="aws2-amazon-s3-connection">
  <unique-id>my-s3-connection</unique-id>
  <region>us-east-1</region>
  <authentication class="aws2-static-credentials-builder">
    <access-key>YOUR_ACCESS_KEY</access-key>
    <secret-key>YOUR_SECRET_KEY</secret-key>
  </authentication>
</connection>
```

### Connection with Custom Endpoint

For use with S3-compatible services (e.g., MinIO, LocalStack):

```xml
<connection class="aws2-amazon-s3-connection">
  <unique-id>localstack-s3-connection</unique-id>
  <region>us-east-1</region>
  <authentication class="aws2-static-credentials-builder">
    <access-key>test</access-key>
    <secret-key>test</secret-key>
  </authentication>
  <custom-endpoint>
    <service-endpoint>http://localhost:4566</service-endpoint>
    <signing-region>us-east-1</signing-region>
  </custom-endpoint>
  <force-path-style-access>true</force-path-style-access>
</connection>
```

### Connection Properties

| Property | Description | Required | Default |
|----------|-------------|----------|---------|
| `region` | AWS region (e.g., us-east-1, eu-west-1) | Yes | - |
| `authentication` | AWS credentials provider | Yes | - |
| `custom-endpoint` | Custom S3 endpoint configuration | No | AWS S3 |
| `force-path-style-access` | Use path-style access for all requests | No | false |
| `client-configuration` | Advanced AWS client configuration | No | - |
| `retry-policy` | Custom retry policy | No | - |

## Operations

All operations are used within the `aws2-amazon-s3-service`:

```xml
<service class="aws2-amazon-s3-service">
  <connection class="aws2-amazon-s3-connection">
    <!-- connection config -->
  </connection>
  <operation class="aws2-amazon-s3-upload">
    <!-- operation config -->
  </operation>
</service>
```

### Upload Operation

Upload message payload to S3.

**Class:** `aws2-amazon-s3-upload`

**Configuration:**

```xml
<operation class="aws2-amazon-s3-upload">
  <bucket>my-bucket</bucket>
  <object-name>path/to/file.txt</object-name>
  <user-metadata-filter class="metadata-filter-impl">
    <!-- Optional: filter metadata to include as user metadata -->
  </user-metadata-filter>
  <canned-object-acl>PublicRead</canned-object-acl>
  <object-metadata>
    <s3-content-type>
      <content-type>application/json</content-type>
    </s3-content-type>
    <s3-server-side-encryption/>
  </object-metadata>
</operation>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `bucket` | S3 bucket name | Yes | Yes |
| `object-name` | S3 object key/path | Yes | Yes |
| `user-metadata-filter` | Filter for message metadata to include | No | - |
| `canned-object-acl` | Predefined ACL (e.g., PublicRead, Private) | No | Yes |
| `object-acl` | Custom ACL configuration | No | - |
| `object-metadata` | List of metadata to set on object | No | - |

**Canned ACL Values:**
- `Private`
- `PublicRead`
- `PublicReadWrite`
- `AuthenticatedRead`
- `BucketOwnerRead`
- `BucketOwnerFullControl`
- `AwsExecRead`

### Download Operation

Download an S3 object to the message payload.

**Class:** `aws2-amazon-s3-download`

**Configuration:**

```xml
<operation class="aws2-amazon-s3-download">
  <bucket>my-bucket</bucket>
  <object-name>path/to/file.txt</object-name>
  <temp-directory>/tmp</temp-directory>
  <user-metadata-filter class="no-op-metadata-filter"/>
</operation>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `bucket` | S3 bucket name | Yes | Yes |
| `object-name` | S3 object key/path | Yes | Yes |
| `temp-directory` | Temporary directory for download | No | java.io.tmpdir |
| `user-metadata-filter` | Filter for extracting user metadata | No | - |

**Notes:**
- User metadata from the S3 object is added to the message metadata
- For `FileBackedMessage`, the file is initialized directly from the downloaded file
- Otherwise, content is copied to the message output stream

### Copy Operation

Copy an object within S3 (basic copy without metadata preservation).

**Class:** `aws2-amazon-s3-copy`

**Configuration:**

```xml
<operation class="aws2-amazon-s3-copy">
  <bucket>source-bucket</bucket>
  <object-name>source/path/file.txt</object-name>
  <destination-bucket>dest-bucket</destination-bucket>
  <destination-object-name>dest/path/file.txt</destination-object-name>
</operation>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `bucket` | Source bucket name | Yes | Yes |
| `object-name` | Source object key | Yes | Yes |
| `destination-bucket` | Destination bucket (defaults to source bucket) | No | Yes |
| `destination-object-name` | Destination object key | Yes | Yes |

**Note:** This operation does NOT preserve server-side-encryption, storage-class, or website-redirect-location. Use `ExtendedCopyOperation` if you need these preserved.

### Extended Copy Operation

Copy an object within S3 with full metadata and tag preservation.

**Class:** `aws2-amazon-s3-extended-copy`

**Configuration:**

```xml
<operation class="aws2-amazon-s3-extended-copy">
  <bucket>source-bucket</bucket>
  <object-name>source/path/file.txt</object-name>
  <destination-bucket>dest-bucket</destination-bucket>
  <destination-object-name>dest/path/file.txt</destination-object-name>
  <object-metadata>
    <s3-content-type>
      <content-type>application/json</content-type>
    </s3-content-type>
  </object-metadata>
  <object-tags>
    <key-value-pair>
      <key>Environment</key>
      <value>Production</value>
    </key-value-pair>
  </object-tags>
</operation>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `bucket` | Source bucket name | Yes | Yes |
| `object-name` | Source object key | Yes | Yes |
| `destination-bucket` | Destination bucket | No | Yes |
| `destination-object-name` | Destination object key | Yes | Yes |
| `object-metadata` | Override/add metadata | No | - |
| `object-tags` | Override/add tags | No | - |

**Features:**
- Automatically retrieves and preserves existing metadata
- Automatically retrieves and preserves existing tags
- Allows overriding specific metadata or tags
- Preserves server-side-encryption and other advanced settings

### Delete Operation

Delete an object from S3.

**Class:** `aws2-amazon-s3-delete`

**Configuration:**

```xml
<operation class="aws2-amazon-s3-delete">
  <bucket>my-bucket</bucket>
  <object-name>path/to/file.txt</object-name>
</operation>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `bucket` | S3 bucket name | Yes | Yes |
| `object-name` | S3 object key to delete | Yes | Yes |

### List Operation

List objects in an S3 bucket with optional filtering.

**Class:** `aws2-amazon-s3-list`

**Configuration:**

```xml
<operation class="aws2-amazon-s3-list">
  <bucket>my-bucket</bucket>
  <prefix>path/to/folder/</prefix>
  <max-keys>1000</max-keys>
  <filter class="size-based-filter">
    <filter-condition class="greater-than">
      <value>1024</value>
    </filter-condition>
  </filter>
  <output-style class="csv-by-metadata">
    <metadata-key>s3-object-list</metadata-key>
    <separator>,</separator>
  </output-style>
</operation>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `bucket` | S3 bucket name | Yes | Yes |
| `prefix` | Filter objects by prefix | No | Yes |
| `max-keys` | Maximum keys per page | No | - |
| `filter` | Additional filtering on results | No | - |
| `output-style` | How to render the list | No | Simple list |

**Output Styles:**
- Default: Simple newline-separated list of object names
- `csv-by-metadata`: CSV format stored in metadata
- `json-array-by-metadata`: JSON array stored in metadata
- Custom implementations available

### Check File Exists Operation

Check if an object exists in S3 (throws exception if not found).

**Class:** `aws2-amazon-s3-check-file-exists`

**Configuration:**

```xml
<operation class="aws2-amazon-s3-check-file-exists">
  <bucket>my-bucket</bucket>
  <object-name>path/to/file.txt</object-name>
</operation>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `bucket` | S3 bucket name | Yes | Yes |
| `object-name` | S3 object key to check | Yes | Yes |

**Note:** This operation throws an exception if the object doesn't exist. Consider wrapping with `exception-handling-service-wrapper` if a missing object is part of your expected workflow.

### Tag Operation

Add or update tags on an S3 object.

**Class:** `aws2-amazon-s3-tag`

**Configuration:**

```xml
<operation class="aws2-amazon-s3-tag">
  <bucket>my-bucket</bucket>
  <object-name>path/to/file.txt</object-name>
  <tag-metadata-filter class="metadata-filter-impl">
    <include-pattern>^tag-.*</include-pattern>
  </tag-metadata-filter>
</operation>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `bucket` | S3 bucket name | Yes | Yes |
| `object-name` | S3 object key | Yes | Yes |
| `tag-metadata-filter` | Filter to select metadata as tags | No | RemoveAllMetadataFilter |

**Notes:**
- Metadata matching the filter will be set as S3 object tags
- If no tags match the filter, no tagging operation is performed

### Get Tag Operation

Retrieve tags from an S3 object and add them to message metadata.

**Class:** `aws2-amazon-s3-get-tag`

**Configuration:**

```xml
<operation class="aws2-amazon-s3-get-tag">
  <bucket>my-bucket</bucket>
  <object-name>path/to/file.txt</object-name>
  <tag-metadata-filter class="metadata-filter-impl">
    <include-pattern>^Environment$</include-pattern>
  </tag-metadata-filter>
</operation>
```

**Properties:**

| Property | Description | Required | Supports %message{} |
|----------|-------------|----------|---------------------|
| `bucket` | S3 bucket name | Yes | Yes |
| `object-name` | S3 object key | Yes | Yes |
| `tag-metadata-filter` | Filter tags to add as metadata | No | All tags |

## Object Metadata

S3 object metadata can be set during upload or copy operations. Available metadata types:

### S3ContentType

Set the content type of the object.

```xml
<s3-content-type>
  <content-type>application/json</content-type>
</s3-content-type>
```

Supports `%message{}` expressions.

### S3ContentEncoding

Set the content encoding.

```xml
<s3-content-encoding>
  <content-encoding>gzip</content-encoding>
</s3-content-encoding>
```

### S3ContentDisposition

Set the content disposition header.

```xml
<s3-content-disposition>
  <content-disposition>attachment; filename="data.json"</content-disposition>
</s3-content-disposition>
```

### S3ContentLanguage

Set the content language.

```xml
<s3-content-language>
  <content-language>en-US</content-language>
</s3-content-language>
```

### S3ServerSideEncryption

Enable server-side encryption (AES-256).

```xml
<s3-server-side-encryption/>
```

### S3HttpExpiresDate

Set the HTTP expires date.

```xml
<s3-http-expires-date>
  <time-to-live>
    <unit>HOURS</unit>
    <interval>24</interval>
  </time-to-live>
</s3-http-expires-date>
```

### S3ExpirationTimeRuleId

Set the expiration time rule ID.

```xml
<s3-expiration-time-rule-id>
  <expiration-time-rule-id>delete-after-30-days</expiration-time-rule-id>
</s3-expiration-time-rule-id>
```

## Access Control Lists (ACL)

### Canned ACLs

Use predefined ACLs for simple access control:

```xml
<canned-object-acl>PublicRead</canned-object-acl>
```

### Custom ACLs

Define fine-grained access control:

```xml
<object-acl class="s3-object-acl">
  <grants>
    <s3-object-acl-grant>
      <grantee class="s3-object-acl-grantee-canonical-user">
        <identifier>canonical-user-id</identifier>
      </grantee>
      <permission>FullControl</permission>
    </s3-object-acl-grant>
  </grants>
</object-acl>
```

**Available Permissions:**
- `FullControl`
- `Read`
- `Write`
- `ReadAcp`
- `WriteAcp`

## Retry Store

Use S3 as a failed message store for retry functionality.

**Class:** `aws2-amazon-s3-retry-store`

**Configuration:**

```xml
<retry-store class="aws2-amazon-s3-retry-store">
  <connection class="aws2-amazon-s3-connection">
    <!-- connection config -->
  </connection>
  <bucket>failed-messages-bucket</bucket>
  <prefix>failed-messages</prefix>
</retry-store>
```

**Properties:**

| Property | Description | Required |
|----------|-------------|----------|
| `connection` | S3 connection | Yes |
| `bucket` | Bucket for storing failed messages | Yes |
| `prefix` | Prefix for organizing failed messages | No |

**Features:**
- Stores message payload as `{prefix}/{msg-id}/payload.blob`
- Stores metadata as `{prefix}/{msg-id}/metadata.properties`
- Stores stack trace as `{prefix}/{msg-id}/stacktrace.txt`
- Supports listing and retrieving failed messages
- Supports deletion of processed messages

## Examples

### Example 1: Upload JSON File to S3 (AWS SDK v2)

```xml
<service class="aws2-amazon-s3-service">
  <connection class="aws2-amazon-s3-connection">
    <unique-id>s3-connection</unique-id>
    <region>us-east-1</region>
    <authentication class="aws2-static-credentials-builder">
      <access-key>${aws.access.key}</access-key>
      <secret-key>${aws.secret.key}</secret-key>
    </authentication>
  </connection>
  <operation class="aws2-amazon-s3-upload">
    <bucket>my-data-bucket</bucket>
    <object-name>data/%message{timestamp}.json</object-name>
    <object-metadata>
      <s3-content-type>
        <content-type>application/json</content-type>
      </s3-content-type>
      <s3-server-side-encryption/>
    </object-metadata>
  </operation>
</service>
```

### Example 2: Download and Process S3 Object

```xml
<service class="aws2-amazon-s3-service">
  <connection class="aws2-amazon-s3-connection">
    <unique-id>s3-connection</unique-id>
    <region>eu-west-1</region>
    <authentication class="aws2-default-credentials-provider"/>
  </connection>
  <operation class="aws2-amazon-s3-download">
    <bucket>input-bucket</bucket>
    <object-name>%message{s3-key}</object-name>
    <user-metadata-filter class="no-op-metadata-filter"/>
  </operation>
</service>
```

### Example 3: Copy Object with Metadata Preservation

```xml
<service class="aws2-amazon-s3-service">
  <connection class="aws2-amazon-s3-connection">
    <unique-id>s3-connection</unique-id>
    <region>us-west-2</region>
    <authentication class="aws2-static-credentials-builder">
      <access-key>${aws.access.key}</access-key>
      <secret-key>${aws.secret.key}</secret-key>
    </authentication>
  </connection>
  <operation class="aws2-amazon-s3-extended-copy">
    <bucket>source-bucket</bucket>
    <object-name>%message{source-key}</object-name>
    <destination-bucket>archive-bucket</destination-bucket>
    <destination-object-name>archive/%message{archive-key}</destination-object-name>
    <object-tags>
      <key-value-pair>
        <key>Archived</key>
        <value>true</value>
      </key-value-pair>
      <key-value-pair>
        <key>ArchivedDate</key>
        <value>%message{current-date}</value>
      </key-value-pair>
    </object-tags>
  </operation>
</service>
```

### Example 4: List and Filter S3 Objects

```xml
<service class="aws2-amazon-s3-service">
  <connection class="aws2-amazon-s3-connection">
    <unique-id>s3-connection</unique-id>
    <region>ap-southeast-2</region>
    <authentication class="aws2-default-credentials-provider"/>
  </connection>
  <operation class="aws2-amazon-s3-list">
    <bucket>data-lake-bucket</bucket>
    <prefix>raw-data/2024/</prefix>
    <max-keys>1000</max-keys>
    <output-style class="json-array-by-metadata">
      <metadata-key>s3-file-list</metadata-key>
    </output-style>
  </operation>
</service>
```

### Example 5: Using S3 with LocalStack for Testing

```xml
<connection class="aws2-amazon-s3-connection">
  <unique-id>localstack-s3</unique-id>
  <region>us-east-1</region>
  <authentication class="aws2-static-credentials-builder">
    <access-key>test</access-key>
    <secret-key>test</secret-key>
  </authentication>
  <custom-endpoint>
    <service-endpoint>http://localhost:4566</service-endpoint>
    <signing-region>us-east-1</signing-region>
  </custom-endpoint>
  <force-path-style-access>true</force-path-style-access>
</connection>
```

### Example 6: Migration Example - Before and After

**Before (AWS SDK v1):**
```xml
<service class="amazon-s3-service">
  <connection class="amazon-s3-connection">
    <unique-id>s3-conn</unique-id>
    <region>us-east-1</region>
    <authentication class="aws-static-credentials-builder">
      <access-key>${aws.key}</access-key>
      <secret-key>${aws.secret}</secret-key>
    </authentication>
  </connection>
  <operation class="amazon-s3-upload">
    <bucket>my-bucket</bucket>
    <object-name>%message{filename}</object-name>
  </operation>
</service>
```

**After (AWS SDK v2):**
```xml
<service class="aws2-amazon-s3-service">
  <connection class="aws2-amazon-s3-connection">
    <unique-id>s3-conn</unique-id>
    <region>us-east-1</region>
    <authentication class="aws2-static-credentials-builder">
      <access-key>${aws.key}</access-key>
      <secret-key>${aws.secret}</secret-key>
    </authentication>
  </connection>
  <operation class="aws2-amazon-s3-upload">
    <bucket>my-bucket</bucket>
    <object-name>%message{filename}</object-name>
  </operation>
</service>
```

### Example 7: Workflow with Upload, Tag, and Archive

```xml
<service-list>
  <services>
    <!-- Upload file -->
    <service class="aws2-amazon-s3-service">
      <connection class="aws2-amazon-s3-connection">
        <unique-id>s3-connection</unique-id>
        <region>us-east-1</region>
        <authentication class="aws2-default-credentials-provider"/>
      </connection>
      <operation class="aws2-amazon-s3-upload">
        <bucket>processing-bucket</bucket>
        <object-name>incoming/%message{filename}</object-name>
        <object-metadata>
          <s3-content-type>
            <content-type>%message{content-type}</content-type>
          </s3-content-type>
        </object-metadata>
      </operation>
    </service>
    
    <!-- Tag the uploaded file -->
    <add-metadata-service>
      <metadata-element>
        <key>tag-ProcessedBy</key>
        <value>InterlokWorkflow</value>
      </metadata-element>
      <metadata-element>
        <key>tag-ProcessedDate</key>
        <value>%message{current-timestamp}</value>
      </metadata-element>
    </add-metadata-service>
    
    <service class="aws2-amazon-s3-service">
      <connection class="aws2-amazon-s3-connection">
        <unique-id>s3-connection</unique-id>
        <region>us-east-1</region>
        <authentication class="aws2-default-credentials-provider"/>
      </connection>
      <operation class="aws2-amazon-s3-tag">
        <bucket>processing-bucket</bucket>
        <object-name>incoming/%message{filename}</object-name>
        <tag-metadata-filter class="metadata-filter-impl">
          <include-pattern>^tag-.*</include-pattern>
        </tag-metadata-filter>
      </operation>
    </service>
    
    <!-- Copy to archive -->
    <service class="aws2-amazon-s3-service">
      <connection class="aws2-amazon-s3-connection">
        <unique-id>s3-connection</unique-id>
        <region>us-east-1</region>
        <authentication class="aws2-default-credentials-provider"/>
      </connection>
      <operation class="aws2-amazon-s3-extended-copy">
        <bucket>processing-bucket</bucket>
        <object-name>incoming/%message{filename}</object-name>
        <destination-bucket>archive-bucket</destination-bucket>
        <destination-object-name>archive/%message{year}/%message{month}/%message{filename}</destination-object-name>
      </operation>
    </service>
  </services>
</service-list>
```

## Best Practices

1. **Use AWS SDK v2 for New Projects**: AWS SDK v2 offers better performance and is actively maintained
2. **Use Message Expressions**: Leverage `%message{key}` expressions for dynamic bucket names and object keys
3. **Metadata Filtering**: Use appropriate metadata filters to control what metadata is stored with S3 objects
4. **Server-Side Encryption**: Enable server-side encryption for sensitive data
5. **Error Handling**: Wrap operations in exception handlers for robust error handling
6. **Connection Reuse**: Share connections across multiple services for better performance
7. **Temp Directory**: Configure appropriate temp directories for download operations
8. **ACL Management**: Use canned ACLs for simple cases, custom ACLs for fine-grained control
9. **Tagging Strategy**: Implement consistent tagging for better object organization and lifecycle management
10. **Testing**: Use LocalStack for local development and testing

## Troubleshooting

### Connection Issues

- Verify AWS credentials are correct
- Check region configuration matches your bucket location
- For custom endpoints, ensure `force-path-style-access` is set to `true`
- Verify network connectivity to S3 endpoints
- Ensure custom endpoint configuration includes both `service-endpoint` and `signing-region`

### Upload/Download Failures

- Check bucket permissions
- Verify object key doesn't contain invalid characters
- Ensure sufficient disk space for downloads
- Review temp directory permissions

### Metadata Issues

- Verify metadata filters are configured correctly
- Check that metadata keys don't contain invalid characters
- Ensure metadata values are properly encoded

### Performance Optimization

- Use appropriate temp directories on fast storage
- Consider using `FileBackedMessage` for large files
- Adjust client configuration for better throughput
- AWS SDK v2 provides better performance out of the box

### Migration Issues

- Update all class names from v1 to v2 format (add `aws2-` prefix)
- Update authentication class from `aws-*` to `aws2-*`
- Custom endpoint configuration structure has changed (use nested `custom-endpoint` element)
- Review any custom client configurations for SDK v2 compatibility

## Differences from AWS SDK v1

### Key Improvements in SDK v2

1. **Better Performance**: Reduced memory footprint and faster execution
2. **Non-blocking I/O**: Support for asynchronous operations
3. **Improved Pagination**: Better handling of large result sets
4. **Modern API**: Cleaner, more intuitive API design
5. **Active Support**: AWS actively maintains and updates SDK v2

### Configuration Changes

- Custom endpoint configuration uses nested structure
- Authentication classes prefixed with `aws2-`
- Some canned ACL values may differ (e.g., `AwsExecRead` in v2)

### When to Use SDK v2

- **New projects**: Always use SDK v2
- **Existing projects**: Migrate when possible for better performance
- **Long-term support**: SDK v2 is the future-proof choice

## Additional Resources

- [AWS S3 Documentation](https://docs.aws.amazon.com/s3/)
- [AWS SDK for Java v2](https://docs.aws.amazon.com/sdk-for-java/latest/developer-guide/home.html)
- [Interlok Documentation](https://interlok.adaptris.net/)
