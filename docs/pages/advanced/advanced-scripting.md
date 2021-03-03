> **Summary:** This page describes how to use scripting services inside your Interlok configuration

As of Interlok __3.9.0__ you can use scripting services to add some custom behaviour in your config.

!> **IMPORTANT** From __4.0.0__ using Java 11, the Nashorn JavaScript engine has been deprecated and is due for removal in Java 15. See the [alternative below](#nashorn-alternative).

## Scripting Services

The scripting services supports arbitary scripting languages (JavaScript, JRuby ...) that are supported by [JSR223](https://jcp.org/aboutJava/communityprocess/pr/jsr223/index.html) a standard scripting API for Java Virtual Machine.

You should take care when configuring this class; it can present an audit trail issue when used in combination with 
[DynamicServiceExecutor](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/4.0-SNAPSHOT/com/adaptris/core/services/dynamic/DynamicServiceExecutor.html) if your script executes arbitrary system commands.
In that situation, all commands will be executed with the current users permissions and may be subject to the virtual machines security manager.

The script is executed and the AdaptrisMessage that is due to be processed is bound against the key "message" and an instance of org.slf4j.Logger is also bound to key "log". These can be used as a standard variable within the script.

## Examples

### ScriptingService (scripting-service)

This service takes a file and executes it. Using JavaScript works out of the box with [interlok-core](https://github.com/adaptris/interlok-core) but JRuby needs [interlok-jruby](https://github.com/adaptris/interlok-jruby).

```xml
<scripting-service>
  <unique-id>scripting-service</unique-id>
  <language>javascript</language>
  <script-filename>file://localhost/./config/script.js</script-filename>
</scripting-service>
```
### EmbeddedScriptingService (embedded-scripting-service)

This service uses an embedded scrip and executes it. Using JavaScript works out of the box with [interlok-core](https://github.com/adaptris/interlok-core) but JRuby needs [interlok-jruby](https://github.com/adaptris/interlok-jruby).

```xml
<embedded-scripting-service>
  <unique-id>scripting-service</unique-id>
  <language>javascript</language>
  <script><![CDATA[
message.addMessageHeader('key', 'value');
message.setContent('Some Payload', 'UTF-8');
]]></script>
</embedded-scripting-service>
```

### JRubyScriptingContainer (jruby-scripting-service)

This service is only available if The optional component [interlok-jruby](https://github.com/adaptris/interlok-jruby) is used.
It executes a JRuby script using JRuby Embed Core Scripting container.
Rather than making use of the JSR223 bindings where things need to be controlled via system properties; this makes use of ScriptingContainer to execute your JRuby scripts which allows more fine-grained control over the behaviour.

```xml
<jruby-scripting-service>
  <unique-id>scripting-service</unique-id>
  <service-script>
    <location>file://localhost/./config/script.js</location>
    <path-type>ABSOLUTE</path-type>
  </service-script>
  <builder class="jruby-default-builder">
    <context-scope>THREADSAFE</context-scope>
    <variable-behaviour>TRANSIENT</variable-behaviour>
    <compile-mode>JIT</compile-mode>
  </builder>
</jruby-scripting-service>
```

## Nashorn Alternative

From __4.0.0__ using Java 11, the Nashorn JavaScript engine has been deprecated and is due for removal in Java 15. If you want to keep using a javascript engine you should consider using [GraalJS](https://github.com/oracle/graaljs) instead.

GraalJS is not directly supported in Interlok but it's really easy to include.
All you have to do is add three jar files ([graal-sdk.jar](https://mvnrepository.com/artifact/org.graalvm.sdk/graal-sdk), [js.jar](https://mvnrepository.com/artifact/org.graalvm.js/js) and [js-scriptengine.jar](https://mvnrepository.com/artifact/org.graalvm.js/js-scriptengine)) in the Interlok lib directory and set a System property (_polyglot.js.nashorn-compat=true_).

### Gradle

If you are using gradle and the recommended [Interlok Parent Gradle](/pages/overview/adapter-gradle.md) you can add GraalJS dependencies as shown below:

```groovy
ext {
  ...
  graalvmVersion='21.0.0.2' // Check and use the latest
}
...
dependencies {
  ...
  // GraalJS dependencies
  interlokRuntime ("org.graalvm.sdk:graal-sdk:$graalvmVersion") { changing=true }
  interlokRuntime ("org.graalvm.js:js:$graalvmVersion") { changing=true }
  interlokRuntime ("org.graalvm.js:js-scriptengine:$graalvmVersion") { changing=true }
  ...
}
```

### System Property

You can add the required compatible system property when starting Interlok via command line

`java -Dpolyglot.js.nashorn-compat=true -jar lib/interlok-boot.jar`

or in the __bootstrap.properties__

`sysprop.polyglot.js.nashorn-compat=true`
