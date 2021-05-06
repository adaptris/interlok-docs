> **Summary:** This page describes how to profile Interlok and inject statistics into New Relic

?> **NOTE** If you don't know what [New Relic][] is then you can blithely ignore  this document.

!> **IMPORTANT** This document is for Interlok version 4.0+

## Installation ##

All Interlok metrics require the __interlok-profiler__ component and it's dependencies to be included in your installation, for New Relic however no further components are necessary.

## Enabling the profiler ##

`com.adaptris:interlok-profiler` uses AOP to fire events when the appropriate methods of Workflow, Producer or Service are triggered. It requires `aspjectjweaver` as a java agent when starting the JVM. The recommendation is to not use the bundled wrapper executables, and to roll your own scripts which can provide the correct startup parameters to the JVM. The aspects themselves are stored in `META-INF/profiler-aop.xml` which means that you need to set the appropriate aspectj system property to enable the aspects. 

An example windows start script that starts Interlok with the javaagent and the AOP file settings.
```
setlocal ENABLEDELAYEDEXPANSION

set CLASSPATH=.
set ADAPTRIS_HOME=C:\Adaptris\Interlok4.0
set JAVA_HOME=C:\Java\Zulu\zulu11\bin

set CLASSPATH=%CLASSPATH%;%INTERLOK_HOME%\lib\*;%INTERLOK_HOME%\config

set ASPECT_OPTIONS=-Dorg.aspectj.weaver.loadtime.configuration=META-INF/profiler-aop.xml

%JAVA_HOME%\java -cp %CLASSPATH% -javaagent:lib/aspectjweaver.jar %ASPECT_OPTIONS% -jar ./lib/interlok-boot.jar
```

### Additional profiler detail ###
If you don't require more technical detail on how the profiler works, skip this section.

The profiler maintains an instance of a JMX MBean per Interlok component; for each and every service, producer and workflow.
Each of those MBeans contains 3 important metrics;
 - AverageNanoseconds - This is the average amount of time this component takes to process a message
 - MessageCount - The number of messages this component has processed
 - FailedMessageCount - The number of messages failed in this component.

You can find the MBeans with the following JMX query;
__com.adaptris:type=Profiler,*__

You can further narrow the results per component type like this for workflows, services or producers;
__com.adaptris:type=Profiler,componentType=workflow,*__
__com.adaptris:type=Profiler,componentType=service,*__
__com.adaptris:type=Profiler,componentType=producer,*__

A further narrowing allows us to specify the unique-id of the component.  Take this example query for a specific workflow;
__com.adaptris:type=Profiler,componentType=producer,id=my-workflow-id__

## Enabling New Relic ##

You may want to follow the latest guide to install the [New Relic Java Agent][]. Essentially, New Relic's javaagent is simply a zipped directory containing all required files to perform metric uploads from a Java process.  New Relic suggest installing there javaagent outside of your Interlok installation, i.e. it is important that the New Relic javaagent is not copied into the Interlok __lib__ directory.

There are 3 further steps to complete the New Relic integration;

1) Modify the newrelic.yml to include your New Relic API key and set the application name to something like "Interlok".

2) Modify your Interlok start script using the one above as a base to include New Relic's javaagent;
```
%JAVA_HOME%\java -cp %CLASSPATH% -javaagent:lib/aspectjweaver.jar %ASPECT_OPTIONS% -javaagent:C:\path-to\newrelic.jar -jar ./lib/interlok-boot.jar
```
Here we have simply added the New Relic javaagent to the last line, do make sure the path to the newrelic.jar is set correctly.

3) Finally we need to add JMX extensions to your New Relic installation.
Adding extensions is actually quite straight forward; create a new directory in the root of your New Relic installation named __extensions__, now crteate as many yml extension files as you want to instruct the New Relic javaagent to scrape metrics from JMX.

### Custom New Relic extensions ###

As mentioned above you'll create an extensions directory at the root of your New Relic installation.  Now you can add as many extension yml files as you wish, the naming of the files is not important as long as the file extension is "yml".  Each yaml file will target an Interlok JMS profiling MBean(s), see the profiling additional information above for further details, check the [New Relic JMX Extension documentation][] or simply use one of the samples below.   

This sample extension named __producer_nanos.yml__ will send all producer average processing times to New Relic

```yml
name: Producer Average Nanos
version: 1.0
enabled: true
jmx:
  - object_name: com.adaptris:type=Profiler,componentType=producer,*
    metrics:
      - attributes: AverageNanoseconds
        type: simple
        root_metric_name: Producer_nanos_{id}
```
The metric name sent to New Relic will be "Producer_nanos_" + the __unique_id__ of the producer component e.g. __Producer_nanos_myProducer__.

The following example will send the number of messages all of your workflows have processed;

```yml
name: Workflow Throughput
version: 1.0
enabled: true
jmx:
  - object_name: com.adaptris:type=Profiler,componentType=workflow,*
    metrics:
      - attributes: MessageCount
        type: monotonically_increasing
        root_metric_name: Workflow_count_{id}
```

## The Metrics ##

Now simply start Interlok and within a couple of minutes you'll start to see Metrics flowing into your New Relic dashboard.

![NewRelic](../../images/profiling/NRDefault.png)

Once you start to see non-web traffic in your dashboard you'll be able to query for the individual metrics;

![NewRelicInterlokMetrics](../../images/profiling/NRAverageNanosWorkflow.png)

[New Relic]: http://newrelic.com
[New Relic JMX Extension documentation]: https://docs.newrelic.com/docs/agents/java-agent/custom-instrumentation/java-agent-custom-jmx-instrumentation-yaml/
[New Relic Java Agent]: https://docs.newrelic.com/docs/agents/java-agent/
