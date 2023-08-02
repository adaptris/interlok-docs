# Interlok Installation #

!> **NOTE:** **Interlok 5.0+ requires Java 17**.

Installation is pretty easy, however due to a change in Java licensing as of 2019 you need to provide your own 64bit JVM.
You have 2 choices for installation;
 - Using our Java based installer
 - Using gradle


## Java based installer

### Unix / Windows / Mac ###

Simply download and follow the instructions from the latest releases page:

[Interlok Releases Page](https://github.com/adaptris/interlok-release/releases/latest)

### Gradle ###

Please see the full gradle installation guide [here](/pages/overview/adapter-gradle)

## Install as a Windows service using Winsw 

If you want to "run as Windows service" then we suggest using something like [winsw](https://github.com/winsw/winsw) to wrap the java process.

We advise to follow their documentation but one way of doing it is as follow:

- Download the appropriate WinsSw.exe (you can rename it if you want) and put it into the Interlok bin directory.

- Add a new file WinsSw.xml (with the same name as the exe file) next to  it with the following content:

```xml
<service>
  <id>interlok</id>
  <name>Interlok</name>
  <description>This service runs Interlok.</description>
  <executable>C:\path\to\Interlok\bin\start-interlok.bat</executable>
  <log mode="reset"></log>
  <logpath>C:\path\to\Interlok\logs</logpath>
</service>
```

- Don't forget to change the executable and logpath paths.
- Run as an administrator: WinsSw.exe install.
- There should now be a service called Interlok.
- You can start and stop this service as any other Windows services.

