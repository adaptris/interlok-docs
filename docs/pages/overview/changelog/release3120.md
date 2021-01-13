## Version 3.12.0 ##

Release Date : 2021-01

The 3.12.0 release is a small release that focused on some dependency upgrades.

### Key Highlights

- Added STS (Security Token Service) support for building AWS (Amazon Web Services) credentials
- Saxon dependency has been upgraded from 9.9.1-7 to 10.3
- Added the ability to set ACL (Access Control List) to AWS S3 upload operations
- The build-parent can now report on additional warnings from -configcheck

### Bugs

'INTERLOK-3177' - Java11 + docker: JMXMP doesn't appear to start.
'INTERLOK-3519' - interlok-mail github actions failing.
'INTERLOK-3527' - StandardHttpProducer - NPE
'INTERLOK-3531' - interlok-cache - Upgrade jackson and httpclient in apache-geode
'INTERLOK-3537' - PAS consumer still seems to require 'durable' flag to be set even with a subscription ID
'INTERLOK-3539' - JRuby - Fix failing build because of CVE-2020-28052
'INTERLOK-3544' - ExtendedCopyOperation is broken when testing against localstack
'INTERLOK-3553' - Copyright date is incorrect

### Improvements

'INTERLOK-3177' - 'Java11 + docker' JMXMP doesn't appear to start.
'INTERLOK-3519' - interlok-mail github actions failing.
'INTERLOK-3527' - StandardHttpProducer - NPE
'INTERLOK-3531' - interlok-cache - Upgrade jackson and httpclient in apache-geode
'INTERLOK-3537' - PAS consumer still seems to require 'durable' flag to be set even with a subscription ID
'INTERLOK-3539' - JRuby - Fix failing build because of CVE-2020-28052
'INTERLOK-3544' - ExtendedCopyOperation is broken when testing against localstack
'INTERLOK-3553' - Copyright date is incorrect
'INTERLOK-3177' - 'Java11 + docker' JMXMP doesn't appear to start.
'INTERLOK-3519' - interlok-mail github actions failing.
'INTERLOK-3527' - StandardHttpProducer - NPE
'INTERLOK-3531' - interlok-cache - Upgrade jackson and httpclient in apache-geode
'INTERLOK-3537' - PAS consumer still seems to require 'durable' flag to be set even with a subscription ID
'INTERLOK-3539' - JRuby - Fix failing build because of CVE-2020-28052
'INTERLOK-3544' - ExtendedCopyOperation is broken when testing against localstack
'INTERLOK-3553' - Copyright date is incorrect
'INTERLOK-3500' - travis-ci -> github actions for codecov.io
'INTERLOK-3510' - SNYK does not handle variables + dependencies from multi-module parents
'INTERLOK-3517' - Mark AS2 as deprecated
