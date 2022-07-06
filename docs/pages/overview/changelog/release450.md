## Version 4.5.0 ##

Release Date : 2022-07-01

The 4.5.0 release is a small release that focused on some dependency upgrades.

### Bug

- 'INTERLOK-3902' - CVE-2021-23413 - Upgrade jszip to 3.10.0
- 'INTERLOK-3900' - CVE-2022-24785 - Upgrade moment.js to 2.29.3
- 'INTERLOK-3899' - UI - Js error when saving the top service collection of a work unit
- 'INTERLOK-3898' - UI - Selenium remote driver dependency should have test scope
- 'INTERLOK-3891' - Switching the UI to use Postgres DB fails with interlok UI 4.4
- 'INTERLOK-3889' - Interlok Kafka - Vulnerability CVE-2021-28165
- 'INTERLOK-3888' - Javadocs - LogMessageService does not say what the default logging-format is
- 'INTERLOK-3886' - UI Config - Typo in Error message when applying config
- 'INTERLOK-3874' - Interlok Build Parent - Non SemVer jar files are renamed badly when copying into the distribution dir 
- 'INTERLOK-3875' - CVE-2021-43859 - Denial of Service - XStream
- 'INTERLOK-3865' - Spotbugs issues after upgrade to 5.0.1

### Improvement

- 'INTERLOK-3868' -  Archive the interlok-csv-json project
- 'INTERLOK-3867' -  Archive the interlok-vertx project
- 'INTERLOK-3873' -  Force SimpleDateFormat where used to be strict
- 'INTERLOK-3863' -  UI Config - Improve the new on progress service collection
- 'INTERLOK-3862' -  XA - Resource name uniqueness
- 'INTERLOK-3860' -  Add Solace/Websphere to LGTM/Snyk
- 'INTERLOK-3834' -  File utils - protocol prefix
- 'INTERLOK-3832' -  UI Config - Remove the Action Button Size user pref
- 'INTERLOK-2931' -  UI API - Upgrade swagger resources
- 'INTERLOK-2866' -  Friendly error when your config cannot be found.
- 'INTERLOK-2824' -  Added a seed based password implementation
- 'INTERLOK-2752' -  %message resolution should have safe versions