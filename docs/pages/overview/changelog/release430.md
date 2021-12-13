## Version 4.3.0 ##

Release Date : 2021-11

### Known Issues

- _2021-12-13_ - Log4j2 vulnerability - CVE-2021-44228 - [Refer to this page concerning Apache Log4j 2 security vulnerabilities](https://logging.apache.org/log4j/2.x/security.html)

### Key Highlights

- There is a new '[Interlok Component Search](https://interlok.adaptris.net/interlok-docs/#/pages/overview/adapter-component-search)' feature in our documentation allowing you to discover all our configurable components
- A new service collection editor has been added to the [Config Page](https://interlok.adaptris.net/interlok-docs/#/pages/ui/ui-config-screens?id=navigating-the-config-page) that changes the nested display of services in the list container (needs the [User Preference](https://interlok.adaptris.net/interlok-docs/#/pages/ui/ui-user-preferences?id=global-preferences) 'enable technical preview features' to be enabled)
- [UI Templates](https://interlok.adaptris.net/interlok-docs/#/pages/ui/ui-templates) now display the list of required optional components to use the given template
- New [documentation page](https://interlok.adaptris.net/interlok-docs/#/pages/ui/ui-auto-register-to-remote) that explains how to auto register an adapter to remote UI Dashboard
- The [Solace](https://github.com/adaptris/interlok-solace) JCSMP has had many [improvements](https://github.com/adaptris/interlok-solace/pull/24), including updates to use their latest API and add advanced connection/session properties; Reworking of the per-message-properties to be resolvable items, so we can use static and dynamic values; and improvements to the async event handler
- A new command line installer is available to download
- New ['proxy' management component](https://github.com/adaptris/interlok-workflow-rest-services/tree/develop/interlok-proxy) that allows you, for example, to have an API endpoint serviced by Interlok and have jolokia enabled
- New ['rabbitmq' optional component](https://github.com/adaptris/interlok-amqp/tree/develop/interlok-rabbitmq) that uses the rabbitmq java client

### Bug

- 'INTERLOK-3851' - When using ROOT.war we get an exception at startup
- 'INTERLOK-3850' -  Jetty Consumer - Possible threading issue when initializing the handlers
- 'INTERLOK-3840' -  Interlok Installer - Garbled characters when using on Mac OS Big Sur
- 'INTERLOK-3806' -  UI Jolokia - Cannot retrieve failed message stacktrace

### Improvement

- 'INTERLOK-3797' -  UI Config Testing modal - improve the metadata inputs so the tab/enter key after entering new md row takes you to the next md input
- 'INTERLOK-2705' -  @NotNull and @NotBlank annotations should have a message
- 'INTERLOK-2603' -  UI Unit Tests - replace PhantomJS as our JavaScript unit testing solution
- 'INTERLOK-3849' -  UI API - Accept encoded password when using the API to save an adapter in the dashboard
- 'INTERLOK-3848' -  Interlok Installer - Implement a command line installer
- 'INTERLOK-3845' -  OAuth - Default http - request timeout
- 'INTERLOK-3844' -  UI Templates - Update existing templates to use the tmpl-optional-components attribute
- 'INTERLOK-3843' -  UI - Clean development.adaptris.net links
- 'INTERLOK-3842' -  Test ExpiringMapCache expiry settings.
- 'INTERLOK-3838' -  Solace - JCSMP - Rewrite async event handler
- 'INTERLOK-3837' -  Generate Sample Work-Units
- 'INTERLOK-3835' -  IBM WMQ - Disabling auto reconnect
- 'INTERLOK-3834' -  File utils - protocol prefix
- 'INTERLOK-3833' -  UI Config - Implement a new service list editor that can be stand alone and with better handling of nested service list
- 'INTERLOK-3831' -  JCSMP Per message properties - resolvable
- 'INTERLOK-3830' -  JCSMP - connection/session properties
- 'INTERLOK-3828' -  Resolvable expressions for files
- 'INTERLOK-3812' -  Interlok Docs - Add new (non-es) 'Interlok component search' to docs home page/new page
- 'INTERLOK-3543' -  Add payload services
- 'INTERLOK-2581' -  UI Config - Optional components template options
- 'INTERLOK-2442' -  UI Projects - improve the user journey for configuring their first variable
- 'INTERLOK-2247' -  UI Config - improve behaviour when c&p a component that's using a variable
- 'INTERLOK-2147' -  Component that auto-registers the "starting" adapter.
- 'INTERLOK-1920' -  UI Config - new user preference - Open config sidebar by default.
- 'INTERLOK-1441' -  Some core classes don't have the apache license
- 'INTERLOK-1270' -  Make adapter output start failure information regardless of startAdapterQuietly flag

