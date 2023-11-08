## Version 5.0.0 ##

Release Date : 2023-11-08

The 5.0.0 release is focused on Interlok supporting Java 17.

### Key Highlights

- This Interlok version has been compiled for Java 17.
- Lots of deprecated things have been removed; please execute --configtest (or use the parent gradle) with an existing 4.9.1 instance to see what might have been removed
- Lots of work has been done to fix Java 17 deprecation warnings within Interlok

### Improvement

- 'INTERLOK-4154' - AMQP - Update to 3.0
- 'INTERLOK-4123' - Payload path encryption - service which allows you to encrypt the contents of a specified path in your file
- 'INTERLOK-4161' - WorkUnit - load the default required variables from inside the work-unit jar and list them as required metadata in the UI
- 'INTERLOK-4160' - new annotation that can direct the uI to search for required variables
- 'INTERLOK-4158' - Load required variables from the work-unit jar files variables file, directly into the Ui key-value-pair set.
- 'INTERLOK-4045' - upgrade all our Testing projects to work with Java17
- 'INTERLOK-3294' - upgrade interlok-cassandra dependencies 
- 'INTERLOK-2975' - Closing down while connection-retrying improvements
- 'INTERLOK-3990' - Review code and functionality for AWS S3 for SDK 2.
- 'INTERLOK-4175' - UI - Replace moment.js
- 'INTERLOK-4163' - Documentation - revise advanced section
- 'INTERLOK-4174' - UI Work Unit - Hide work unit project tabs which are not relevant
- 'INTERLOK-4204' - Investigate compatability Xalan Cirrus lookup client compatability with v5
- 'INTERLOK-3994' - AWS SDK2 - Commons - Review code and functionality for the commons AWS SDK 2 library.
- 'INTERLOK-3991' - AWS SDK2 - KMS - Review code and functionality for AWS KMS for SDK 2.
- 'INTERLOK-4196' - Interlok-JSON - Bump jwtVersion from 0.11.5 to 0.12.2
- 'INTERLOK-4187' - Flyway - flyway jar should be in lib dir and not in UI war
- 'INTERLOK-4182' - VCS Git - Upgrade to JGit 6.7+
- 'INTERLOK-4205' - Change artefact downloader url to use the new URL