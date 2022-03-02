## Version 4.4.0 ##

Release Date : 2021-03-02

The 4.4.0 release is a small release that focused on some dependency upgrades.

### Information

Log4j provides support for JSR 223 scripting languages to be used in some of its components. As of Log4j 2.17.2 the languages to be supported must be specified as a comma separated list in the log4j2.Script.enableLanguages system property. Please refer to the [Apache manual](https://logging.apache.org/log4j/2.x/manual/configuration.html#Scripts) for the latest advice.

### Bug

- 'INTERLOK-3875' - CVE-2021-43859 - Denial of Service - XStream upgrade
- 'INTERLOK-3865' - Fixing Spotbugs issues after upgrade to 5.0.1

### Improvement

- 'INTERLOK-3868' - Archive the interlok-csv-json project
- 'INTERLOK-3867' - Archive the interlok-vertx project
- 'INTERLOK-3873' - Force SimpleDateFormat where used to be strict
- 'INTERLOK-3863' - UI Config - Improve the new on progress service collection
- 'INTERLOK-3862' - XA - Resource name uniqueness
- 'INTERLOK-3860' - Add Solace/Websphere to LGTM/Snyk
- 'INTERLOK-3834' - File utils - protocol prefix
- 'INTERLOK-3832' - UI Config - Remove the Action Button Size user pref
- 'INTERLOK-2931' - UI API - Upgrade swagger resources
- 'INTERLOK-2866' - Friendly error when your config cannot be found.
- 'INTERLOK-2824' - Add a seed based "password" implementation
- 'INTERLOK-2752' - message resolution should have safe versions
