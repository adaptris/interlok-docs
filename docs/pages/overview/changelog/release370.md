## Version 3.7.0 ##

Release Date : 2018-02-05

### Key Highlights

- The UI Config page has been changed to allow it be 'project aware'.
- UI Variable substitutions are now supported via the project setup and the settings editor
- The UI Config sidebar now promotes new components via versioned components lists
- MS Azure OAuth supports authentication via client-secret
- Support added for jackson-jq
- Internal ActiveMQ has been upgraded to latest-stable

### Bugs

 - `INTERLOK-264` - Two Instances appear in Dashboard after restarting adapter
 - `INTERLOK-1481` - Adapter depends on log4j and log4j2
 - `INTERLOK-1642` - AS2 fails to find the RecipientID in the document
 - `INTERLOK-1693` - UI - Can't edit DataInputParameter properties
 - `INTERLOK-1853` - Loading a config from custom git can be very slow
 - `INTERLOK-1860` - UI fails to auto-discover local adapter
 - `INTERLOK-1892` - Javadoc 404 for SecurityHandlerWrapper
 - `INTERLOK-1923` - schema does not work with interlok-boot.jar
 - `INTERLOK-1959` - Config Test passes with Producer as Service
 - `INTERLOK-1968` - UI Config - MultiProducerWorkflow Standalone Producers list allows any service to be added
 - `INTERLOK-1984` - UI Config - Test component feature isn't working correctly - js error
 - `INTERLOK-1985` - Opening xml popup from the Message Mertics Table and Metadata statistics Table widgets doesn't work in Edge and Chrome
 - `INTERLOK-1986` - interlok-salesforce: OrderedBatchProducerService causes Stackoverflow on close
 - `INTERLOK-1987` - interlok-salesforce: Doesn't package required properties in ./resources/sql/jar
 - `INTERLOK-1991` - XStream 1.4.10 logs a warning on startup
 - `INTERLOK-1992` - sonicmf bootstrap.properties.url doesn't seem to handle logging
 - `INTERLOK-1993` - Log4jConfigurator assumes log4j config is file based and local.
 - `INTERLOK-1995` - Unsupported MQ options in NativeConsumer give unhelpful error message
 - `INTERLOK-2017` - About link in login page and error page is broken.
 - `INTERLOK-2021` - AS2 Fails to decrypt in some instances
 - `INTERLOK-2022` - Improper Handling Of Encodings
 - `INTERLOK-2060` - TypedStatementParameter convert-null = false doesn't pass through null
 - `INTERLOK-2061` - UI Projects - save project label problem
 - `INTERLOK-2064` - UI Projects - xpaths not generated when you upload a config xml into your project
 - `INTERLOK-2066` - Remove interlok-ui-swagger-codegen from the optional component page
 - `INTERLOK-2067` - UI Config - Settings sidebar test panel has errors if you start page without an active adapter
 - `INTERLOK-2075` - Memory leak when using FilebackedMessageFactory

### Improvements

 - `INTERLOK-1356` - Add SSL support for MQTT connection
 - `INTERLOK-1383` - UI Config - Add Information to empty containters to tell users what to do
 - `INTERLOK-1390` - Upgrade internal ActiveMQ to latest-stable
 - `INTERLOK-1486` - Warning when apply config to a remote URL
 - `INTERLOK-1508` - Use AdapterBuilder.createAdapter(xml) insead of AdapterRegistry.createAdapter(xml)
 - `INTERLOK-1579` - Add a URLEncode "modal" somewhere
 - `INTERLOK-1736` - Swagger import should make use of jetty-routing-service in 3.6.4
 - `INTERLOK-1776` - Deprecate the use of jakarta-oro
 - `INTERLOK-1795` - UI Config Project-aware - create a module for management of sets of property lists
 - `INTERLOK-1812` - Cannot test a vcs profile w/o saving it.
 - `INTERLOK-1817` - com.adaptris.core.socket should move to optional?
 - `INTERLOK-1821` - UI Config sidebar - Impl a new 'versioned' list of components in the 'byGroup' list
 - `INTERLOK-1828` - Add a "ConnectedService" interface to mark services that contain connections
 - `INTERLOK-1829` - Add a new overloaded AdapterComponentChecker#applyService()
 - `INTERLOK-1831` - AdaptrisConnection#cloneForTesting()
 - `INTERLOK-1837` - UI Config Project-aware - adapt the settings editor to allow the user to select inputs required for substituted.
 - `INTERLOK-1839` - UI Config Project-aware - Impl a feature to save/export the project-aware context
 - `INTERLOK-1867` - Tests always fail under java9
 - `INTERLOK-1883` - UI Config Component Sidebar - add a user pref to toggle 'show the settings editor' after a drop component event
 - `INTERLOK-1933` - [UI] Add support for Locale + TimeZone as drop downs.
 - `INTERLOK-1951` - Add support for jackson-jq (as an alternative to JOLT).
 - `INTERLOK-1952` - UI Config Project-aware - Expose config-project-store location to a ui system properties
 - `INTERLOK-1974` - RetryMessageErrorHandler should have an MBean for UI control purposes
 - `INTERLOK-1975` - Update knockout and jquery js lib
 - `INTERLOK-1983` - Remove support for log4j1
 - `INTERLOK-1989` - Add MS Azure OAuth implementation that supports authentication via client-secret
 - `INTERLOK-1994` - Add supporting X12 services
 - `INTERLOK-1997` - IronMQ is now paid for; need to switch to using MOCKs only
 - `INTERLOK-2010` - Deploy interlok-service-tester javadocs to development.adaptris.net
 - `INTERLOK-2011` - Examples should follow the javadoc classifier convention
 - `INTERLOK-2014` - Update install-builder to use m:classifier="javadocs"
 - `INTERLOK-2019` - as2-message-builder needs to be smarter about building AS2 / AS2MDN messages
 - `INTERLOK-2020` - Config & LicenseTaglet should extend an AbstractTaglet (from service-tester)
 - `INTERLOK-2023` - Commit-MDN needs to be smarter when checking dispositions
 - `INTERLOK-2024` - Merge branch INTERLOK-1836 into develop and clean code
 - `INTERLOK-2031` - interlok-hpcc: Update format to allow implementations
 - `INTERLOK-2035` - Add a Regexp MetadataValueMatcher
 - `INTERLOK-2036` - Add com.adaptris.failover.FailoverBootstrap to interlok-boot
 - `INTERLOK-2037` - Add variables set selection when applying a config (project) to an adapter.
 - `INTERLOK-2045` - Add inline doc in the config project modal
 - `INTERLOK-2071` - Support 6.x Elastic search API
 - `INTERLOK-2073` - Test and document Interlok - WMQ with SSL
 - `INTERLOK-1916` - jms-producer should optionally exclude all headers matching the pattern ^JMS_.*
 - `INTERLOK-1977` - JdbcMapInsert should allow wrapping of column names
 - `INTERLOK-2012` - as2-commit-message renders Message-ID as Message-Id
 - `INTERLOK-2015` -> 0.7.9
 - `INTERLOK-2016` - -XX:-UseSplitVerifier when running unit tests -> -noverify
 - `INTERLOK-2032` - UI: Csv -> CSV for friendly ness
 - `INTERLOK-2040` - UI: Projects Bring back the import option
 - `INTERLOK-2062` - UI Optional - update icons for oauth and new interlok projects