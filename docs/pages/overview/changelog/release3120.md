## Version 3.12.0.1 ##

Release Date : 2021-02-11

The 3.12.0.1 release resolves a single issue; It does not have an installer, and only affects the following artifact jars since they are built from the same multi-module repository: _interlok-boot.jar, interlok-client.jar, interlok-client-jmx.jar, interlok-common.jar, interlok-core.jar, interlok-core-apt.jar, interlok-logging.jar_

If you're affected by this issue, then you should update your dependency tree to use `com.adaptris:interlok-core:3.12.0.1-RELEASE`

- 'INTERLOK-3702' - retry-via-jetty setting reporting-endpoint does not work

## Version 3.12.0 ##

Release Date : 2021-01-26

The 3.12.0 release is a small release that focused on some dependency upgrades.

### Known Issues

- _2021-01-27_ - There is an issue with the [DatabaseConnection](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/3.12-SNAPSHOT/com/adaptris/core/jdbc/DatabaseConnection.html), during this release the field [testStatement](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/3.12-SNAPSHOT/com/adaptris/core/jdbc/DatabaseConnection.html#setTestStatement-java.lang.String-) was marked as Deprecated, but it was left as a required field. This means you can not blank this deprecated field. You can however, leave a test statement in and have 'Always Validate Connection' set to false (which is the default). This issue is being tracked in 'INTERLOK-3580'.

### Key Highlights

- Added STS (Security Token Service) support for building AWS (Amazon Web Services) credentials
- Saxon dependency has been upgraded from 9.9.1-7 to 10.3
- Added the ability to set ACL (Access Control List) to AWS S3 upload operations
- The build-parent can now report on additional warnings from -configcheck

### Bugs

- 'INTERLOK-3177' - Java11 + docker: JMXMP doesn't appear to start.
- 'INTERLOK-3519' - interlok-mail github actions failing.
- 'INTERLOK-3527' - StandardHttpProducer - NPE
- 'INTERLOK-3531' - interlok-cache - Upgrade jackson and httpclient in apache-geode
- 'INTERLOK-3537' - PAS consumer still seems to require 'durable' flag to be set even with a subscription ID
- 'INTERLOK-3539' - JRuby - Fix failing build because of CVE-2020-28052
- 'INTERLOK-3544' - ExtendedCopyOperation is broken when testing against localstack
- 'INTERLOK-3553' - Copyright date is incorrect
- 'INTERLOK-3562' - UI Config - Settings Editor Change Type dropdown take all modal width instead of just half

### Improvements

- 'INTERLOK-218' - Mark TestStatement as deprecated in DatabaseConnection
- 'INTERLOK-3520' - UI - Bump jetty to 9.4.35.v20201120 jackson to 2.12.1 and flyway to 7.3.0
- 'INTERLOK-3521' - UI - Bump maven-resources-plugin from 3.1.0 to 3.2.0
- 'INTERLOK-3528' - Possible performance bottleneck in creation of new XPath instances
- 'INTERLOK-3534' - UI - Bump spring to 4.3.30 and hibernate to 5.4.25.Final
- 'INTERLOK-3541' - Core - Upgrade good.cer to fix TestCertificateHandler > testGoodCertificateExpiry
- 'INTERLOK-3549' - UI - Bump jersey to 2.33, bouncycastle to 1.68, xerces to 2.12.1 and mockito to 3.7.0
- 'INTERLOK-3550' - Update components that are Deprecated for the 3.12.0 release to be Deprecated for 4.0.0 release
- 'INTERLOK-2724' - Run interlok using graalvm
- 'INTERLOK-2873' - MetadataComparison as a condition
- 'INTERLOK-3299' - interlok-azure-cosmosdb: Auth should be a Request Interceptor
- 'INTERLOK-3403' - Upgrade things from mockito:1.10.19 to mockito-core:3
- 'INTERLOK-3481' - Google pubsub GRPC upgrade breaks.
- 'INTERLOK-3485' - Test: XSLT 2/3 - And multi-payload
- 'INTERLOK-3497' - Extend interlok-verify-report to use available ConfigurationCheckers
- 'INTERLOK-3511' - interlok-aws-s3: Add the ability to set the objectAcl on upload operation
- 'INTERLOK-3512' - UI Version Upgrade - update Bootstrap select and tour to latest version
- 'INTERLOK-3522' - Bump Saxon from 9.9.1-7 to 10+
- 'INTERLOK-3525' - Add support STS for AWS credentials to assume IAM roles
- 'INTERLOK-3526' - Add unique-id to javax.validation.checker output
- 'INTERLOK-3530' - UI - Bump flyway-core from to 7.3.2, hibernate-validator to 6.1.7.Final and swagger-v3 to 2.1.6
- 'INTERLOK-3532' - interlok-service-tester-wiremock: When using helper wiremock tests take a long time to complete
- 'INTERLOK-3533' - interlok-service-tester-wiremock: Wiremock helper doesn't use service.tester.working.directory
- 'INTERLOK-3555' - Optional component url in the pom file point to the wrong doc pages
- 'INTERLOK-3561' - PoolingWorkflow that doesn't have a ThreadPool
- 'INTERLOK-3570' - UI - Test the ui database switch using a MariaDB