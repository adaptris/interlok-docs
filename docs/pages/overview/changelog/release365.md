## Version 3.6.5 ##

Release Date : 2017-10-11

### Key Highlights

- A new Salesforce API Browser page that will aid you in building Interlok Config that interacts with a Salesforce API.
- The Config page has a new sidebar feature, that can be used to add components to Config via drag and drop.
- Improved OAUTH support for salesforce / google cloud / MS azure
- New Easy CSV / JSON insert via JDBC
- Service list supports 'forward-search' style branching

### Bugs

- `INTERLOK-1743` - MetadataElement values may be "" but not null
- `INTERLOK-1745` - REST API returns 200 OK even if channel is not found
- `INTERLOK-1768` - UI Config - the settings editor metadata preview doesn't handle shared services
- `INTERLOK-1781` - UI - Adapter cannot be removed from dashboard if its having trouble to connect
- `INTERLOK-1809` - UI Config - MetadataElement list don't render corrrectly in the settings modal
- `INTERLOK-1810` - vcs-git not in runtime-libraries.zip
- `INTERLOK-1815` - Interlok-UI shouldn't count services when doing the class descriptor tests.
- `INTERLOK-1818` - UI Config sidebar - errors from dnd add appear in model window, not main window
- `INTERLOK-1825` - amazon-s3-connection should support a "region"
- `INTERLOK-1826` - UI Config - Rendering Issue when input field hint password is in lower case.
- `INTERLOK-1833` - VCS-Profile doesn't allow you to specify a branch
- `INTERLOK-1834` - UI Config - Drag and Drop Services not working
- `INTERLOK-1835` - UI Config - re-ordering a service created via the sidebar creates an unwanted copy
- `INTERLOK-1844` - LogMessageService never logs the payload unless include-events=true
- `INTERLOK-1848` - Both javax.mail.jar + javax.mail-glassfish.jar in distribution
- `INTERLOK-1849` - default-mail-consumer fails for null subjects.
- `INTERLOK-1858` - Interlok still doesn't report unchecked exceptions on startup
- `INTERLOK-1872` - TemplateServiceImplTest testListService test failure on jenkins
- `INTERLOK-1894` - AdvancedRabbitMqImpl doesn't mirror the getters/setters from RMQConnectionFactory exactly

### Improvements

- `INTERLOK-1453` - UI - Isolate the UI code that generates the class definitions and implementation lists
- `INTERLOK-1780` - UI "Add Adapter" Checkbox for no validation on add
- `INTERLOK-1788` - Allow interlokuidb.properties properties to be overriden by system properties.
- `INTERLOK-1789` - Allow empty/missing username + password in interlokuidb.properties
- `INTERLOK-1819` - UI Config sidebar - the 'add via sidebar' needs to support the adding of shared components
- `INTERLOK-1820` - UI Config sidebar - using templates with wizards, ignores the wizard and just adds
- `INTERLOK-1850` - Support XSLT 3.0 by upgrading Saxon
- `INTERLOK-1877` - Switch InstallAnywhere executables to use interlok-boot.jar
- `INTERLOK-1118` - Remove use of @GenerateBeanInfo where required.
- `INTERLOK-1275` - Doc Section/Page Request: "HTTP cookbook"
- `INTERLOK-1456` - UI Config - Add components by dragging from open side panel
- `INTERLOK-1604` - RawMailConsumer should have a header-handler
- `INTERLOK-1621` - UI Config - Improve the DynamicServiceLocator settings editor usage
- `INTERLOK-1689` - service-list should support 'forward-search' style branching
- `INTERLOK-1727` - Add the ability to open from file system a config with x-include zip file
- `INTERLOK-1771` - JSON Aggregator implementation
- `INTERLOK-1772` - Non Public jars should be marked as optional not compile dependencies
- `INTERLOK-1777` - Cleanup half removed features from the UI
- `INTERLOK-1779` - CSV->JDBC insert service
- `INTERLOK-1782` - Better 'auth' detection for vcs-git
- `INTERLOK-1786` - dynamic-jmx-service to execute the same JMX operation against different JMXServiceURL
- `INTERLOK-1791` - JSON->JDBC Insert
- `INTERLOK-1793` - MessageTypeTranslator allows setting property type
- `INTERLOK-1797` - UI - Salesforce - Make the salesforce public and add the ability to create service xml from it
- `INTERLOK-1799` - Add MS Azure OAUTH implementation
- `INTERLOK-1800` - Separate GCloud OAuth Provider from PubSub project
- `INTERLOK-1802` - Mobile UI - build the home page and add ui adapters page
- `INTERLOK-1806` - Separate SF oauth from apache-http
- `INTERLOK-1814` - Move com.adaptris.transport.* -> OFTP package
- `INTERLOK-1851` - Make MailboxClient return an Iterator<MimeMessage>
- `INTERLOK-1852` - Add a S3-Delete / Copy operation
- `INTERLOK-1857` - JdbcMapInsert should have a "descriptor" file
- `INTERLOK-1864` - adp-core-apt is broken in java 9
- `INTERLOK-1870` - Replace StandardBootstrap for Java 9
- `INTERLOK-1896` - Simpler way to generate Basic Authorization header
- `INTERLOK-1881` - UI Billboards/Videos - Promote the salesforce/sidebar-dnd via welcome splash/video-docs
- `INTERLOK-1891` - UI Billboards - Update the season event billboard css image.
