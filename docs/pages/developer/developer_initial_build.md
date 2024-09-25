
> **Summary:** Getting started as a developer.

This document will walk you through the first steps of getting access to the code bases, tools and then building the binaries.

## Prerequisites.

You will need the following installed and then configure the _PATH_ (assuming windows) and _JAVA_HOME_.

 - Gradle - 7.6.2
 - Java OpenJDK - 17

## Accessing the code bases

With Interlok being open source software, you can access most of the Interlok codebases in github.  We have the core Interlok engine [here](https://github.com/adaptris/interlok) and the full list of Interlok optional components [here](https://github.com/adaptris). 

## Building the binaries

Clone or download the [interlok-core](https://github.com/adaptris/interlok) codebase.
In the root of the project you'll find the gradle.build file and then a few sub-projects, each of which have their own build files.

Command line navigate to the root of the cloned/downloaded project directory and assuming you have set your _PATH_ correctly with the gradle install directory you can simply execute a build;

```cmd
> gradle build
```
Alternatively you can use the gradle wrapper included in the project;
```
> gradlew.bat build
```

Now check the _./build/_ directory for reports and final binaries.

The _build_ task will compile the source and unit test code, run the unit tests, generate a coverage report, run spotbugs and finally generate the jar binary.

Some of the other notable gradle tasks you can run are (and of course chain together);
- gradle clean -- Will remove the build directory.
- gradel jar -- Will skip the tests and reports and simply create the jar binary
- gradle test -- Will execute the unit tests and generate a test report
- gradle check -- Will execute the unit tests and generate the unit test and coverage reports
- gradle dependencyCheckAnalyze -- Will check the dependencies for security vulnerabilities


