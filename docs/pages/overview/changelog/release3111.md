## Version 3.11.1 ##

Release Date : 2020-11-30

### Key Highlights

- The UI Config Settings Editor inputs now have a 'code autocomplete' feature for % properties
- Interlok Runtime improvements include:
    - The ALTPW password variant has now been marked as deprecated, and the support of it will be removed for Interlok 4.0
    - New PooledSplitJoinService which has been designed to improve performance on very very large split messages
    - Added (a prototype) One Drive consumer and producer that allows for getting and putting of individual files from/to One Drive.
    - configcheck has been improved to generate a deprecated report similar to the one used for config validation without parsing the console deprecated warnings
    - New REST based failed message retrier

### Bugs

- 'INTERLOK-3450' - ALTPW: password variant should be marked as deprecated
- 'INTERLOK-3455' - JMS Creating durable subscriber with subscription name.
- 'INTERLOK-3458' - Wrong GUI validation of Idoc Producer against Idoc consume connection instead of Idoc produce connection
- 'INTERLOK-3459' - Green percent sign not displayed in GUI for field lookup-name within dynamic-shared-service
- 'INTERLOK-3461' - FileFilterBuilder doesnt' support Filters with default constructors.
- 'INTERLOK-3462' - Alternative password styles are not supported by the UI
- 'INTERLOK-3471' - UI - Importing widgets in the runtime page doesn't save them if nothing else is done in the page
- 'INTERLOK-3477' - UI - The Generate Services button from the DysnamicServiceLocator is not available for the DysnamicServiceExecutor
- 'INTERLOK-3484' - Json validator dups
- 'INTERLOK-3490' - PluggableJdbcConnection + HikariCP fails to pass configuration checks
- 'INTERLOK-3503' - UI - self referenced vars improvements - varsub infinite loop

### Improvements

- 'INTERLOK-2716' - Reference Implementation JMS Bridge
- 'INTERLOK-3043' - UI Log Monitor - add feature to 'clear visible log'
- 'INTERLOK-3146' - UI Config Settings Editor - give the settings inputs a 'code autocomplete' feature for % properties
- 'INTERLOK-3269' - Official doc site update
- 'INTERLOK-3287' - New extended validation reporting for deprecated items
- 'INTERLOK-3401' - UI Config - Improve 'add component' list, so when filtering by 'shared' then shared-components are listed first
- 'INTERLOK-3415' - JCSMP - Alternative authentication
- 'INTERLOK-3417' - JCSMP - Transaction handling
- 'INTERLOK-3424' - Improve performance of PoolingSplitJoin for large splits
- 'INTERLOK-3426' - CSV to JSON_LINES service
- 'INTERLOK-3440' - Create a builder for get-and-cache-oauth-token service for json payload with custom headers from metadata
- 'INTERLOK-3447' - GenericOauthToken should propagate the "http code"
- 'INTERLOK-3448' - JCSMP - Configurable ack window
- 'INTERLOK-3456' - Unit tests - Embedded brokers
- 'INTERLOK-3465' - REST based triggered failed message retrier
- 'INTERLOK-3468' - Promote 'interlok-manual' as the formal documentation page.
- 'INTERLOK-3472' - Conditional loops - StopProcessingService
- 'INTERLOK-3473' - Tidy up the solace project
- 'INTERLOK-3474' - interlok-mail: send-email-attachment should allow body contentType to be set
- 'INTERLOK-3501' - Add a new listener to JettyRetry that allows delete
- 'INTERLOK-3508' - ConfigChecker - SharedComponents doesn't support nested services
- 'INTERLOK-2330' - MS Graph - Impl prototype for pulling and pushing to One Drive.
- 'INTERLOK-2331' - MS Graph - interlok-azure - Office365 consumer and producer
- 'INTERLOK-2332' - MS Graph - extend the OneDrive consumer/producer, so documents can now be retrieved and converted into other formats
- 'INTERLOK-748' - JMS translators - be able to specify an encoding?
- 'INTERLOK-3436' - Update resolvable expressions Jsonpath documentation
- 'INTERLOK-3449' - UI - Upgrade xtream, common-io, snakeyaml, mockito and maven dependency-check
- 'INTERLOK-3460' - Xpath Service doesn't support attribute nodes
- 'INTERLOK-3464' - UI: Bump flyway to 7.0.2
- 'INTERLOK-3469' - UI - Bump junit from 4.13 to 4.13.1
- 'INTERLOK-3475' - UI - Bump hibernate-validator to 6.1.6.Final, flyway-core to 7.0.4, commons-pool2 to 2.9.0 and javax.el to 3.0.1-b12
- 'INTERLOK-3476' - UI - Upgrade gridstack.js and d3.js
- 'INTERLOK-3478' - UI - Upgrade raphael.js to 2.3.0
- 'INTERLOK-3483' - UI - Upgrade to jetty 9.4.33.v20201020, Mockito 3.5.15 and Swagger v3 to 2.1.5
- 'INTERLOK-3486' - UI - Upgrade shiro to 1.7.0 and flyway to 7.1.1
- 'INTERLOK-3491' - Double deprecation warning reporting in DeprecationChecker
- 'INTERLOK-3492' - UI - update links so they all point to the correct (new) documentation pages
- 'INTERLOK-3493' - US style Date formatting (interlok-docs docsify)
- 'INTERLOK-3495' - UI - Upgrade jetty to 9.4.34.v20201102
- 'INTERLOK-3496' - Doc - Add docs about the new ConfigDeprecated annotation

