Interlok's core component provides the base functionality to give you a start for your integration solution.  Many other components can be bolted on to provide extended functionality or custom handling for vendor specific technologies.  You can find a list of additional components [here](/pages/user-guide/adapter-optional-components).
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

## Build a 3.12 Interlok instance

So the above guide will build you the latest v4 version of Interlok, but what if you wanted the latest v3 version (3.12.0.3 at the time of writing).

Here's what you would do:

Simply edit ext section from the 'build.gradle' file 
```
ext {
  interlokVersion = '3.12.0-RELEASE' 
  interlokUiVersion = interlokVersion
  interlokParentGradle = "https://raw.githubusercontent.com/adaptris/interlok-build-parent/develop/v3/build.gradle"
```
The above changes, point to the v3 build parent file, and also change the Interlok version to 3.12.0

Also, changes the dependencies section in the 'build.gradle' file:
```
dependencies {
  interlokRuntime ("com.adaptris:interlok-core:3.12.0.3-RELEASE") { changing=true }
```
This will make sure the core version is at the latest 3.12.0.3 version

Then you would do exactly like before
Windows:
```
> gradle clean assemble
> (cd ./build/distribution && java -jar lib/interlok-boot.jar)
```
Note, that I used gradle assemble rather than gradle build, as the tests for this example project will fail with v3 jars, but we can still build and execute interlok without running the tests.

## Further reading / More options

For more information and documented additional gradle options (including how to specify the Interlok version) see our parent gradle docs [here](https://github.com/adaptris-labs/interlok-build-parent).
For more details on the sample project we've cloned for this exercise go [here](https://github.com/adaptris-labs/build-parent-json-csv/tree/docker-image).