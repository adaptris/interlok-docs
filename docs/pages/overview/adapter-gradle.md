!> **NOTE:** **Interlok 5.0+ requires Gradle 7.6.1**.

Interlok's core component provides the base functionality to give you a start for your integration solution.  Many other components can be bolted on to provide extended functionality or custom handling for vendor specific technologies.  You can find a list of additional components [here](/pages/user-guide/adapter-optional-components-search) or  [here](/pages/user-guide/adapter-optional-components).
Each component essentially consists of an additional Interlok Java library and it's required dependent Java libraries.  Therefore making sure you add all of the required dependant libraries can be a challenge.  The standard way to to build your Interlok instances without fear of dependency management is to use our gradle builds.

This guide will walk you through creating both a standalone and optionally a docker Interlok instance with the optional components you require.

## Setup

The steps are very simple with most of the difficulties having been handled for you.  Simply clone [this](https://github.com/adaptris-labs/build-parent-json-csv/tree/docker-image) sample project to your local filesystem.   You can clone the project using either GIT clone or simply downloading the zip file.

Windows:
```
> git clone https://github.com/adaptris-labs/build-parent-json-csv.git --config core.autocrlf=input
> git checkout docker-image
```
Linux/Mac
```
> git clone https://github.com/adaptris-labs/build-parent-json-csv.git
> git checkout docker-image
```

If you're interested in building a docker image from this guide and you have used GIT clone as above, then you will need to make sure you switch to the "docker-image" branch.  If however you have the zip file from the link above then simply read on.

## Dependencies

Now simply edit the gradle.build file, specifically the dependencies section.

```groovy
dependencies {
  interlokRuntime ("com.adaptris:interlok-json:$interlokVersion") { changing=true }
  interlokRuntime ("com.adaptris:interlok-csv:$interlokVersion") { changing=true }
  interlokRuntime ("com.adaptris:interlok-csv-json:$interlokVersion") { changing=true }
  interlokRuntime ("com.adaptris:interlok-apache-http:$interlokVersion") { changing=true }

  interlokJavadocs group: "com.adaptris", name: "interlok-apache-http", version: "$interlokVersion", classifier: "javadoc", changing: true, transitive: false
  interlokJavadocs group: "com.adaptris", name: "interlok-json", version: "$interlokVersion", classifier: "javadoc", changing: true, transitive: false
  interlokJavadocs group: "com.adaptris", name: "interlok-csv", version: "$interlokVersion", classifier: "javadoc", changing: true, transitive: false
  interlokJavadocs group: "com.adaptris", name: "interlok-csv-json", version: "$interlokVersion", classifier: "javadoc", changing: true, transitive: false
}
```
Here we have a list of components we want to include both for runtime and the documentation.   The list currently consists of;
 - interlok-json
 - interlok-csv
 - interlok-csv-json
 - interlok-apache-http

Add or remove the required components.

Finally edit or replace your Interlok configuration files in the directory ./src/main/interlok/config

## Build your standalone instance

On your command line navigate to the root of your checked out project and use the built in gradle executable to build.

Windows:
```
> gradlew.bat clean build
```
Linux/Mac
```
> gradlew clean build
```
Your full Interlok installation including required additional components will be pulled together and found in the ./build/distribution directory.  From that directory you can now simply run Interlok;
```
> java -jar ./lib/interlok-boot.jar
```

## What if the build fails?

During the build several verification steps are executed, each should generate a report in the **./build/reports/** directory.  If the file is empty it means no errors were found.  Otherwise you should see the detail causing your build failure.

One of these verification tasks will run the service tester if you have set up tests for your workflows.  The configuration for service-tester can be found at **./src/test/interlok**.

!> **The default project has a sample service-tester configuration, which MUST be removed or changed to your service-test configuration.**

## Build your docker instance

Simply use your local docker installation to create your image;
```
> docker build --tag "your/tag-name" .
```
Then run it;
```
> docker run -it --rm -p8080:8080 your/tag-name
```
After a moment to allow Interlok to complete it's startup you can log-in to the Interlok web interface at [http://localhost:8080](http://localhost:8080)

## Build a v4 Interlok instance

If you want the latest v4 version of Interlok (4.9.0 at the time of writing) follow the guid in the [v4 doc](https://interlok.adaptris.net/interlok-docsv4/#/pages/overview/adapter-gradle)

## Build a v3 Interlok instance

If you want the latest v3 version of Interlok (3.12.0.3 at the time of writing) follow the guid in the [v3 doc](https://interlok.adaptris.net/interlok-docsv3/#/pages/overview/adapter-gradle).

## Further reading / More options

For more information and documented additional gradle options (including how to specify the Interlok version) see our parent gradle docs [here](https://github.com/adaptris/interlok-build-parent).
For more details on the sample project we've cloned for this exercise go [here](https://github.com/adaptris-labs/build-parent-json-csv/tree/docker-image).
