> **Summary:** This is here to help you get started writing your own services and what not.

The simplest scenario is to have a local adapter installation and make sure all the jars in the `lib` directory are present in your classpath when you come to compile your classes (either by having a script that sets up the classpath, or making sure `${adapter}/lib/*.jar` is included into your classpath when you invoke the `javac` task.

However, that doesn't need to be the case; all our public artefacts are available in our [maven compatible repository](https://nexus.adaptris.net/nexus/content/repositories/releases/). This means that, you can use your preferred build tool to manage dependencies be it gradle, maven or otherwise.

?> **TIP** An example quickstart project on github : [https://github.com/adaptris/interlok-custom-component-example](https://github.com/adaptris/interlok-custom-component-example)

Unless you're in an environment where you must use an alternative build toolchain; we recommend that you use gradle since this gives you good flexibility along with standardised conventions. If you just want to get started hacking code then go straight to our github example project : [https://github.com/adaptris/interlok-custom-component-example](https://github.com/adaptris/interlok-custom-component-example).

There are a few features tucked into our gradle sample project that will greatly help with your new components integration into the interlok platform; which you should definitely be aware of if you choose to use another build tool but still want tight integration.

### The version report
```
> gradlew.bat clean jar
```
The above command will generate the jar file artefact which will include an "adaptris-version" file within the "META-INF" directory.

This version file is very useful whenever you want to see a list of Interlok components and their versions currently installed into your instance.  For example, when connecting to your instance through the web UI you can click for more instance information on the dashboard page which will list a component and version report, including your new component should you make sure this "adaptris-version" file exists as described above.

An example of the file:
```
#Thu, 13 Jul 2023 11:22:46 +0100

component.name=My Custom Interlok Component
groupId=io.github.adaptris
artifactId=interlok-custom-component-example
build.version=5.0-SNAPSHOT
build.date=2023-07-13
build.info=gradle
```

### Component searching

```
> gradlew.bat clean jar
```
The above command will also create a file instead your new component jar file in the "META-INF/adaptris" directory named "component.properties".

This file aids integration engineers while building interlok instance configuration to find your components through a search box.  The file simply includes a list of fully qualified packaged components which would include any consumers, producers, services or workflows you have created.

### Friendly component naming

```
> gradlew.bat clean jar
```

The above command will also create the "XStreamAlias.properties" file, which will include a list of fully qualified classes that can be configured directly within Interlok configuration.

The point of the file allows Interlok to interrogate that list of java classes so that we can keep track on a map of classes to aliases.  An example of a class might be "com.adaptris.samples.EchoProducer" while it's alias might be "my-echo-producer".  This allows us when configuring Interlok to use the alias within XML rather than the classes fully qualified package name; much friendlier. 

### Additional benefits of using our sample project

```
> gradlew.bat clean check
```

This command at the root of the sample project directory will run all of your tests, producing a test report with detail of any failures.  It will also run a coverage report detailing line and branch coverage percentage.  
The reports can be found in the "build/reports" directory.

## A short excursion into the whys and wherefores of dependency management

Like the argument about whether or not your VCS is better than my VCS. What matters the most is that you aren't using CVS (where CVS is the equivalent of making all the jars in `{adapter}/lib` present on the classpath.). Without dependency management there is a very real possibility that you end up in the equivalent of _DLL Hell_ where you have jackson-databind-2.10.1.jar trying to use jackson-core-2.9.jar for some of its baseline operations.

Previously we used ant+ivy to handle dependency management; we've moved to gradle for almost everything now. Examples remain in the public github example repository for the different build tools that we've built components with.

