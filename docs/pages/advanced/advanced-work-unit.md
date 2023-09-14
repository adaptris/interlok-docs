> **Summary:** This page describes how to configure Interlok Work Unit

## What is it? ##

A Work Unit is simply a service-list configuration and any supporting files your services require bundled into a jar file. That is to say you may have a complex and / or often used set of services that you find yourself copying into multiple installations of Interlok and you now want to make that list of services more modular, maintainable and reusable.

The Work Unit allows you to black box that process making it easier for the next person to re-use your process (set of services).

## Configuring your Work Unit service-list ##

The first thing is to build your work-unit.xml. This should contains a service-list with your configuration.

That's it, it's just a service list. An example;

```xml
<service-collection class="service-list">
  <services>
    <service class="log-message-service">
      <unique-id>log-message-service</unique-id>
      <log-level>DEBUG</log-level>
    </service>
  </services>
</service-collection>
```

Sometimes your `service-list`` will require additional files; for example if you're configuring a transform then you'll need the XSL file. Sometimes the additional resource required will be remote, perhaps you're serving a transform over HTTP. But other times you want the resource locally packaged with your configuration. In this case your Work Unit jar file will contain your service-list configuration and another supporting file like an XSL transform named "my-transform.xsl".

In these cases it's important that in your work unit's service list you refer to the packaged resource file like this using the workunit: URL handler; The URL is in the form of:

`protocol:work-unit-name!/path/to/file` e.g. -> `workunit:my-work-unit!/my-transform.xsl`.

__work-unit-name__ is the artifactId of your Work Unit defined in the Work Unit __adaptris-version__ file.

```xml
<service-collection class="service-list">
  <services>
    <xml-transform-service>
      <unique-id>transform-service</unique-id>
      <url>workunit:my-work-unit!/my-transform.xsl</url>
    </xml-transform-service>
  </services>
</service-collection>
```

## Using the Work Unit ##

Once you have your work unit Jar file and it's dropped into your Interlok lib directory (make sure your re-start Interlok) you can then edit your main configuration adding a new service. If you have a `service-list`` file packed in that my-work-unit.jar jar file named __work-unit.xml__, then inside your main Interlok configuration you can refer to your work unit's service list simply like this;

### Simple use case ##

```xml
<work-unit-service>
  <unique-id>work-unit-service</unique-id>
  <!-- Jar name without .jar -->
  <work-unit-name>my-work-unit</work-unit-name>
  <!-- Xml name without .xml. Optional, default to work-unit -->
  <xml-config-name>work-unit</xml-config-name>
</work-unit-service>
```

### Variables Substitutions ###

A Work Unit jar file can have variables.properties along with the work-unit.xml files that can be used to replace tokens in the config. To use these variable properties, you will have to use `work-unit-variable-set`. Let say you want to use the variables in the __variables.properties__ file within your Work Unit.

```xml
<work-unit-service>
...
  <work-unit-variable-set>
    <name>variables</name>
  </work-unit-variable-set>
...
</work-unit-service>
```

You can add multiple variable set with the latest one taking precedences. Let say you also have a __variables-test.properties__ file.

```xml
<work-unit-service>
...
  <work-unit-variable-set>
    <name>variables</name>
  </work-unit-variable-set>
  <work-unit-variable-set>
    <name>variables-test</name>
  </work-unit-variable-set>
...
</work-unit-service>
```

The other way to do variables substitutions is to provide key value pairs in the work unit service like:

```xml
<work-unit-service>
...
  <key-value-pair-variable-set>
    <variables>
      <key-value-pair>
        <key>key1</key>
        <value>Value 1</value>
      </key-value-pair>
      <key-value-pair>
        <key>key2</key>
        <value>Value 2</value>
      </key-value-pair>
    </variables>
  </key-value-pair-variable-set>
...
</work-unit-service>
```

Where _key1_ and _key2_ is a variable replacement key in the __work-unit.xml__ file.

## Building a Work Unit ##

The Work Unit is a jar file with a __work-unit.xml__ and other configuration files in it. The Work Unit jar also need a file called __adaptris-version__ in a __META-INF__ directory. The __adaptris-version__ content should be like:

```properties
component.name=My Work Unit
component.description=My work unit that does something
component.type=work-unit
groupId=com.adaptris
artifactId=my-work-unit
```

!> **WARNING**  _component.name_, _component.type_, _groupId_ and _artifactId_ are mandatory.

?> **NOTE** The best way to build your Work Unit jar is to use gradle and have the __work-unit.xml__ and the __variables.properties__ in an Interlok type project.

You can follow the sample project [my-work-unit][]

With a command line prompt run: `gradle clean build`

The __build.gradle__ file will package the project in the right way and will create and fill the __adaptris-version__ file accordingly. The __gradle.properties_ file is where you can specify the _componentName_, _componentDesc_, _organizationName_ and _organizationUrl_.

The _artifactId_ is the project directory name but can also be customised in the __settings.gradle__ (which is optional) file:

`rootProject.name = "my-work-unit"`

## Documenting a Work Unit ##

If you use the example __build.gradle__ file from [my-work-unit][] to build your Work Unit and you have a __README.md__ file at the root of the Work Unit project, it will package in the Work Unit jar. The content of the __README.md__ file will be available in the Interlok UI when adding a `work-unit-service` to explain what the Work Unit is doing.


[my-work-unit]: https://github.com/adaptris/interlok-work-unit/tree/develop-v4/sample/my-work-unit