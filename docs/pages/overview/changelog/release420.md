## Version 4.2.1 ##

### Interlok Core

Release Date : 2021-10-04

The 4.2.1 (Core) release resolves a single issue; It does not have an installer, and only affects the following artifact jars since they are built from the same multi-module repository: _interlok-boot.jar, interlok-client.jar, interlok-client-jmx.jar, interlok-common.jar, interlok-core.jar, interlok-core-apt.jar, interlok-logging.jar_

If you're affected by this issue, then you should update your dependency tree to use `com.adaptris:interlok-core:4.2.1-RELEASE`

- ['782'](https://github.com/adaptris/interlok/issues/782) - interlok-boot.jar gives inconsistent results depending on platform

### Interlok Service Tester

Release Date : 2021-09-14

The 4.2.1 (Service Tester) release resolves a single issue; It does not have an installer, and only affects the following artifact jars since they are built from the same multi-module repository: _interlok-service-tester.jar, interlok-service-tester-json.jar, interlok-service-tester-wiremock.jar, interlok-service-tester-xml.jar_

If you're affected by this issue, then you should update your dependency tree to use `com.adaptris:interlok-service-tester:4.2.1-RELEASE`

- 'INTERLOK-3839' - Service Tester failing with Unsupported Operation

## Version 4.2.0 ##

Release Date : 2021-09-03

### Known Issues

- _2021-09-08_ - There is an issue when using a file-payload-provider inside a service-test. When tests with that provider are being executed, they result in the error 'java.lang.UnsupportedOperationException'. This issue is being tracked in 'INTERLOK-3839'.
- _2021-09-24_ - There is an issue with the InterlokLauncher (inside interlok-boot). Depending on the platform you are running on, the InterlokLauncher may load jars in a different order (on Windows it's 'order alphabetically', on docker (alpine image) it's whatever you want sort order). This issue is being tracked in ['782'](https://github.com/adaptris/interlok/issues/782).

### Key Highlights

- The UI Config Page has had the following improvements:
  - Pagination features on the channel-list, workflow-list and service-list containers
  - Filtering features have been added to those collection containers
  - The loading time of large configurations has been cut down
- Interlok AWS S3 now allows for custom object ACLs to be set during upload operations
- Service Tester now supports testing of services within conditions
- Service Tester has been improved to allow binary files in a test-case


### Bug
- 'INTERLOK-3836' - UI Service Tester - Issue with loading the config service list used when adding a Test
- 'INTERLOK-3829' - UI Config Templates - wmq connection template results in javascript errors
- 'INTERLOK-3824' - UI Config - Settings modal expanded doc error on some services
- 'INTERLOK-3822' - ApacheHTTP - Error on empty response payloads
- 'INTERLOK-3816' - Metadata comparators don't work as operators
- 'INTERLOK-3807' - Interlok Installer - Unable to install interlok 4.0.0 using openjdk version 13.0.2
- 'INTERLOK-3713' - Service Tester - issue using .xls file with a file-payload-provider in a test-case

### Improvement

- 'INTERLOK-3827' -  Oauth - Apache HT|TP Client proxy
- 'INTERLOK-3826' -  interlok-aws-s3: Add the ability to set Custom Object ACLs when uploading
- 'INTERLOK-3825' -  JMS - Unregistering clients
- 'INTERLOK-3823' -  Apache HTTP configurable config builder
- 'INTERLOK-3821' -  JMS - Best practice guide
- 'INTERLOK-3818' -  Reuse operationTimeout within the ShutdownHandler
- 'INTERLOK-3802' -  Interlok Installer - Update the usage of interlok-parent-builder
- 'INTERLOK-3796' -  Update build.gradle config for Gradle 7
- 'INTERLOK-3790' -  Reconfigure dependabot for github native
- 'INTERLOK-3788' -  UI Config - Improve performance of the config page
- 'INTERLOK-3786' -  UI Config - Add filtering features to the pageable containers
- 'INTERLOK-3785' -  UI Config - Add pagination features to the channel-list, workflow-list and service-list containers
- 'INTERLOK-3781' -  Rest - Package naming for sub projects
- 'INTERLOK-3775' -  Ensure the xstream alias is shown in the javadocs
- 'INTERLOK-3538' -  Workflow Rest Service - Definition yaml file always return http for the servers url even when using https
- 'INTERLOK-3330' -  ProduceExceptionHandler Deprecate?
- 'INTERLOK-3064' -  ServiceTester doesn't support services inside conditions (if/switch etc).
- 'INTERLOK-929' -  UI Login page - page doesn't work when already logged in
