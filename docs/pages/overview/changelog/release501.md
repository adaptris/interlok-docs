## Version 5.0.1 ##

Release Date : 2024-02-05

The 5.0.1 release is a small release and is mainly focused on dependency upgrades.

### Improvement

- 'INTERLOK-4309' - JMX-JMS Does not work, need put the add-opens on interlok-bootsrap
- 'INTERLOK-4285' - MimePartSelectorToMetadata has been added to to interlok core
- 'INTERLOK-3301' - Work has been completed on some optional components so that Junit tests can be run in parallel
- 'INTERLOK-4249' - OffsetTimestampGenerator now allows expessions such as %message{XXXX}
- 'INTERLOK-4219' - [interlok-triggered](https://github.com/adaptris/interlok-triggered) is now a public unlicensed project
- 'INTERLOK-4220' - Added input parameter support for xml transform services
- 'INTERLOK-4179' - Config Comments - extend the 'comments' element to individual services and shared services.
- 'INTERLOK-3993' - Added support for [AWS SDK2 - SNS](https://github.com/adaptris/interlok-aws/tree/develop/interlok-aws2-sns)
- 'INTERLOK-3992' - Added support for [AWS SDK2 - SQS](https://github.com/adaptris/interlok-aws/tree/develop/interlok-aws2-sqs)