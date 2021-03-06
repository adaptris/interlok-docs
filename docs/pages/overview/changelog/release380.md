## Version 3.8.0 ##

Release Date : 2018-08-13

This release requires Java 8; Java 7 is no longer supported. Additionally there were some artefact name changes which are documented in [optional components](/pages/user-guide/adapter-optional-components).

!> **IMPORTANT** Use interlok-boot.jar instead of adp-core.jar when running directly from the commandline; also adp-core.jar has been renamed to interlok-core.jar

### Key Highlights

- We have upgraded a lot of our libraries and projects which were Ant based have now been moved to Gradle.
- It's important to note that this Interlok version has been compiled for Java 8 and above.
- To enforce a clean break, all artefact names have been changed from adp-[component] to interlok-[component].
- Cache services have been migrated into Interlok
- There is now a new optional component to access ElasticSearch via their "High-level java REST client"
- Failover TCP mode auto-discovery
- Every optional component now has published Javadocs

### Bugs

 - `INTERLOK-1878` - Log extract from a failed message doesn't match the failed message...
 - `INTERLOK-2252` - Upgrade to derby 10.14.2.0+
 - `INTERLOK-2261` - Update shiro to 1.4.0
 - `INTERLOK-2300` - Sort out the javadocs for Interlok Kafka Optional Component
 - `INTERLOK-2303` - Upgrade quartz and c3p0 in UI pom
 - `INTERLOK-2305` - if-the-otherwise embedded service-list does not display nice in the UI
 - `INTERLOK-2311` - UI Projects - Null pointer exception when loading setting with var + text
 - `INTERLOK-2318` - UI Login - misspelling on page 'Pasword'
 - `INTERLOK-2320` - UI - Upgrade bouncycastle to 1.60
 - `INTERLOK-2321` - Core - Upgrade bouncycastle to 1.60
 - `INTERLOK-2325` - edi-xml-stream-service doesn't cope with escaped fields (composite)
 - `INTERLOK-2334` - xml-edi-service does not output empty fields
 - `INTERLOK-2349` - Issue with HTTP responses, when splitting messages

### Improvements

 - `INTERLOK-1509` - Add redis "com.adaptris.cache" implementation
 - `INTERLOK-2268` - Apache Ignite support
 - `INTERLOK-2272` - Migrate cache interface into interlok
 - `INTERLOK-2273` - Create cache wrapper around ExpiringMap
 - `INTERLOK-2274` - Create interlok-cache project for eh-cache
 - `INTERLOK-2276` - Migrate cache services into interlok
 - `INTERLOK-2315` - Upgrade ehcache project to ehcache 2.10.5
 - `INTERLOK-2354` -  gcloud pubsub requires retesting
 - `INTERLOK-425` - Refactor interlok-opt/ehcache to use JSR107
 - `INTERLOK-2072` - Switch to using the ElasticSearch "Highlevel java REST client"
 - `INTERLOK-2090` - Failover TCP mode auto-discovery
 - `INTERLOK-2176` - Shouid all Javadocs for every optional project be published?
 - `INTERLOK-2215` - Migrate github candidates to gradle
 - `INTERLOK-2228` - UI User Prefs - Improve the way we store and handle the user preferences
 - `INTERLOK-2230` - UI - ConsumerMonitor Widget
 - `INTERLOK-2231` - Update FsConsumerMonitor to return generic getType to remove override
 - `INTERLOK-2260` - Upgrade the interlok artifact downloader to use Spring boot 2.x
 - `INTERLOK-2278` - Use nexus lucene search to list the optional components in the UI
 - `INTERLOK-2279` - Add a new method getArtifactIdentifiers() to AdapterManager
 - `INTERLOK-2286` - Add subscriber group support to Kafka
 - `INTERLOK-2292` - interlok-csv: Create an Iterable OrderedCsvMapReader
 - `INTERLOK-2293` - interlok-csv: CSV metadata splitter
 - `INTERLOK-2297` - Rename all adp- artifacts to interlok-
 - `INTERLOK-2302` - %message{} resolution should support resolving the message-unique-id.
 - `INTERLOK-2314` - interlok-csv-json: JSON to CSV Add the ability to control header inclusion
 - `INTERLOK-2324` - Update snapshot release to 3.8-SNAPSHOT
 - `INTERLOK-2326` - interlok-service-tester: Gradle Plugin
 - `INTERLOK-2335` - interlok-apache-http: Expose more Client Builder options
 - `INTERLOK-2347` - interlok-gcloud-pubsub: Bump google-cloud-pubsub from 0.20.0-beta to 1.37.1
 - `INTERLOK-2353` - Remove FsConsumerMonitor Widget
 - `INTERLOK-2356` - interlok-hpcc: Log every command output line processed
 - `INTERLOK-2283` - UI - Create mockups for settings editor improvements (object lists)
 - `INTERLOK-2289` - UI API - add delete/patch operations for adapters (where key=name, or db-id)
 - `INTERLOK-2291` - UI Optional Components - add the correct link for all the opt comp javadocs
 - `INTERLOK-2295` - Update to xercesImpl 2.12
 - `INTERLOK-2298` - Update references of adp- to interlok- and dependencies on 3.7 to 3.8
 - `INTERLOK-2299` - UI Optional Components - decide what to do about the dead links for javadocs
 - `INTERLOK-2322` - Remove the legacy config store from the configuration page
 - `INTERLOK-2342` - Change direct dependencies text in optional components
 - `INTERLOK-2343` - New Icons required for optional page
 - `INTERLOK-2344` - Upgrade guava to 26.0-jre
 - `INTERLOK-2345` - interlok-jruby # advanced-builder should have a jruby-home
 - `INTERLOK-2346` - Upgrade spring to 4.3.18.RELEASE
 - `INTERLOK-2351` - Upgrade jacoco to 0.8.1
