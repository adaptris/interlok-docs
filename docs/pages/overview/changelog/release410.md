## Version 4.1.0 ##

Release Date : 2021-06-22


### Key Highlights

- A [new interlok-jdbc component](https://github.com/adaptris/interlok-ds/tree/develop/interlok-jdbc) that aims to simplify the syntax when [writing SQL statements](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-jdbc/4.1.0B1-RELEASE/com/adaptris/interlok/jdbc/package-summary.html), part of its goal is to make statement-parameters redundant.
- The [interlok-build-parent project](https://github.com/adaptris/interlok-build-parent) has been promoted from [adaptris-labs](https://github.com/adaptris-labs) to the [adaptris github organisation](https://github.com/adaptris).
- [Interlok service tester](https://github.com/adaptris/interlok-service-tester) has been improved so each test you configure can have a default [globally defined 'MainSource'](https://github.com/adaptris/interlok-service-tester/pull/114), making it easier to setup and re-configure.
- The [Interlok service tester UI page](https://interlok.adaptris.net/interlok-docs/#/pages/ui/ui-service-tester) now supports opening and publishing projects from VCS, like how the [UI Config Page](https://interlok.adaptris.net/interlok-docs/#/pages/ui/ui-version-control) works.
- The Interlok UI now allows adding a new ([interlok-jolokia](https://github.com/adaptris/interlok-jolokia) management enabled) adapter on the dashboard page using a [http jolokia url](https://interlok.adaptris.net/interlok-docs/#/pages/advanced/advanced-jolokia).
- [Added JSON path service](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-json-streaming/4.1.0B1-RELEASE/com/adaptris/core/json/streaming/JsonPathStreamingService.html) that uses [JSON Surfer](https://github.com/jsurfer/JsonSurfer) to parse [JSON as a stream](https://github.com/adaptris/interlok-json/tree/develop/interlok-json-streaming) and extract data using JSON path syntax.
- A [new ftp-recursive-consumer](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/4.1.0B1-RELEASE/com/adaptris/core/ftp/FtpRecursiveConsumer.html) that will recursively descend into any sub directories it finds to consume files.
- The UI Widgets that display static data have been removed from the [widgets page](https://interlok.adaptris.net/interlok-docs/#/pages/ui/ui-widgets), and their data has been relocated to the [UI dashboard](https://interlok.adaptris.net/interlok-docs/#/pages/ui/ui-dashboard) information modal.
- We now offer the ability to publish metrics to [Datadog](https://interlok.adaptris.net/interlok-docs/#/pages/advanced/advanced-profiler-datadog) and [NewRelic](https://interlok.adaptris.net/interlok-docs/#/pages/advanced/advanced-new-relic-profiling_v4)

### Bug

- 'INTERLOK-3803' - Installer : MAC installer doesn't chmod +x bin/start-interlok
- 'INTERLOK-3801' - Swagger Codegen - Vulnerabilities in swagger-parser, httpclient-osgi and handlebars
- 'INTERLOK-3799' - UI: Open Local Project doesn't work with relative paths.
- 'INTERLOK-3794' - UI Config - Test component modal is broken with javascript error \(Uncaught SyntaxError: Unable to parse bindings\)
- 'INTERLOK-3782' - interlok-json-streaming causes classpath issues with the UI
- 'INTERLOK-3777' - UI - Swagger Codegen vulnerabilities
- 'INTERLOK-3735' - Rest metrics - NPE
- 'INTERLOK-3304' - Unckecked Exceptions in FsConsumer - hang.

### Improvement

- 'INTERLOK-3795' - UI Config Settings Editor - allow Javadoc content to be pulled from field as well as setter methods
- 'INTERLOK-3756' - XpathMetadataService does not support expressions
- 'INTERLOK-3784' - UI Config - Template wizard 'Generate unique identifier fields' should be false by default.
- 'INTERLOK-3783' - Promote interlok-build-parent from adaptris-labs to adaptris github organisation
- 'INTERLOK-3781' - Rest - Package naming for sub projects
- 'INTERLOK-3780' - Profiler - Datadog
- 'INTERLOK-3779' - UI Widgets - Remove static platform widget and put the info in the dashboard page
- 'INTERLOK-3771' - Update Custom Component Example to 4.0.0.
- 'INTERLOK-3770' - UI - Remove the Profiler Monitor page as we are not going to maintain it anymore.
- 'INTERLOK-3768' - Newrelic metrics - rework
- 'INTERLOK-3767' - UI External API - Remove deprecated endpoints
- 'INTERLOK-3764' - Profiler - WorkflowID
- 'INTERLOK-3763' - Profiler - Remove ActivityMap
- 'INTERLOK-3762' - Profiler - Research timeslices
- 'INTERLOK-3761' - Profiler - Remove UDP support
- 'INTERLOK-3757' - Add a MultiItemXpathQuery that renders a node-list properly
- 'INTERLOK-3749' - interlok-elastic has a dependency on apache-csv
- 'INTERLOK-3726' - Gaps in prometheus metrics
- 'INTERLOK-3711' - Update retry-store-write-message to store stack trace
- 'INTERLOK-3710' - UI - Support Jolokia http request in the UI
- 'INTERLOK-3599' - interlok-licensing: Add support for environment variables
- 'INTERLOK-3588' - FtpConsumer - Add the posibility to consume files from subfolders
- 'INTERLOK-3524' - License should also have a ConfigurationChecker
- 'INTERLOK-3467' - org.apache.httpcomponents.client5:httpclient5 is now a thing.
- 'INTERLOK-3333' - JsonPath on large JSON
- 'INTERLOK-2930' - Add option for Kinesis with Java SDK rather than KPL
- 'INTERLOK-2758' - JDBCCaptureService statement should build statement parameters automatically
- 'INTERLOK-2671' - UI Service Test - The service test page should support vcs and auto save
- 'INTERLOK-2550' - UI Version Upgrade - update canvg js to latest version
- 'INTERLOK-2491' - UI Config - improve the settings for the EmbeddedScriptingService
- 'INTERLOK-2219' - Service-Tester - New Test Source - globally defined
- 'INTERLOK-2006' - UI API - merge the features of interlok-web-service-restful into the ui api
