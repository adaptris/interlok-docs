## Version 4.6.0 ##

Release Date : 2022-10

### Key Highlights

- [interlok-elastic](https://github.com/adaptris/interlok-elastic) now has an initial implementation of the elastic search 7 SDK named [interlok-elastic-sdk](https://github.com/adaptris/interlok-elastic/tree/develop/interlok-elastic-sdk). This has been introduced as the elastic High Level Rest API is deprecated now in favour of the SDK API.
- [interlok-azure](https://github.com/adaptris/interlok-azure) has had many improvements; including added support for the search parameter in the O365MailConsumer and improvements to working with attachments from the multi payload message.
- The UI [Component Search](https://interlok.adaptris.net/interlok-docs/#/pages/ui/ui-interlok-component-search) has been improved so it doesn't require a connection to a hosted server to work, it has been refactored to use html, js and json instead of an elastic search server.

### Bug

- 'INTERLOK-3932' - Build Parent - Fails if a service-test.xml file exist with no tests
- 'INTERLOK-3919' - Interlok Json - CVE-2011-5034
- 'INTERLOK-3918' - Service Tester - Vulnerability CVE-2022-2048
- 'INTERLOK-3901' - CVE-2021-41182 CVE-2021-41183 CVE-2021-41184 - Upgrade jQuery UI to 1.13.1
- 'INTERLOK-3896' - UI Log Monitor - Exception after adapter UID changed

### Improvement

- 'INTERLOK-3975' - Elastic bulk - Batch Window
- 'INTERLOK-3936' - Interlok Azure Mail - Add attachment metadata
- 'INTERLOK-3935' - CVE - Fix interlok-aws CVE-2022-34917
- 'INTERLOK-3934' - CVE - Fix interlok-pdf CVE-2022-40146
- 'INTERLOK-3933' - Interlok Installer - Use the new base-filesystem zip file
- 'INTERLOK-3930' - Weekly dependency uppgrades
- 'INTERLOK-3928' - Dependencies Upgrade - Bump mockito to 4.8.0 and more
- 'INTERLOK-3926' - Jackson-dataformat needs bumping
- 'INTERLOK-3925' - AWS SQS SNS - Support SQS groupId and SNS message attribute
- 'INTERLOK-3924' - Slf4j - Bump slf4jVersion to 2.0.0
- 'INTERLOK-3921' - Azure Mail -  Support the search param to the O365MailConsumer.
- 'INTERLOK-3912' - SQS - Synchronous sending
- 'INTERLOK-3910' - update interlok-verify-report dependances, release, update parent build
- 'INTERLOK-3907' - Impl latest ES SDK
- 'INTERLOK-3906' - Work units - improve/plan how to use variables with workunits
- 'INTERLOK-3904' - Create a new Metadata Join Service
- 'INTERLOK-3884' - license cmd tool - hand over to chris / document
- 'INTERLOK-3813' - UI Component Search - update the page so it doesn't use the elastic search server
- 'INTERLOK-3920' - Documentation - Datadog
- 'INTERLOK-2985' - UI Config - settings editor variable token selector scroll bar can be 'off screen' when token row is large

