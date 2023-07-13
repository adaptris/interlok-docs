> **Summary:** GA guide for Java developers who want to work with Interlok profiling events for your own monitoring/alerting system.

## Starting the profiler

Before we get into the technical bits, let us show you how to start an instance of Interlok with the profiler.

You'll need the Interlok profiler component which can be included into your Interlok instances gradle build like this;
```groovy
interlokRuntime ("com.adaptris:interlok-profiler:4.8.0-RELEASE:")
```

Including this component will auto-magically pull the required aspectj dependencies.


When running the profiler it is always suggested to create your own script to launch the Interlok process.  Essentially we need to start the Java process with a javaagent, with the profiling configuration.  Here is a windows batch script (start-interlok-with-profiler.bat) that does the necessary;
```
setlocal ENABLEDELAYEDEXPANSION

set CLASSPATH=.
set INTERLOK_HOME=C:\Adaptris\3.10
set JAVA_HOME=C:\Java\jdk\bin

set CLASSPATH=%CLASSPATH%;%INTERLOK_HOME%\lib\*;%INTERLOK_HOME%\config

set ASPECT_OPTIONS=-Dorg.aspectj.weaver.loadtime.configuration=META-INF/profiler-aop.xml

%JAVA_HOME%\java -cp %CLASSPATH% -javaagent:lib/aspectjweaver.jar %ASPECT_OPTIONS% -jar ./lib/interlok-boot.jar
```
There are two important parts to this script, both of which are Java JVM switches.  The first is the use of the __-javaagent__ and the second is the setting of the following environment property __-Dorg.aspectj.weaver.loadtime.configuration=META-INF/profiler-aop.xml__.  

If you drop this batch file into the root of your Interlok installation,  you should only need to change the __JAVA_HOME__ and the __INTERLOK_HOME__ properties to match your correct paths.  There is one more final thing to check however, the final line specifies a jar file named __aspectweaver.jar__ in the __lib__ directory of your Interlok installation.  Make sure your script has the same name of the actual aspectweaver jar in your lib directory, just in case the jar file is named something slightly different.

Now we need a new file in your __config__ directory of your Interlok installation named __interlok-profiler.properties__.  The content of this file should be the following;
```
com.adaptris.profiler.plugin.factory=com.adaptris.monitor.agent.InterlokMonitorPluginFactory
com.adaptris.monitor.agent.EventPropagator=JMX
```

## Working with the events

We have greatly improved the developer access to metrics produced by the profiler.  Now you can access all metrics through JMX.

interlok will create an MBean that includes a count of messages processed, the average nanospeed timing and a count of failed messages for each component.  The MBean interface can be found in the [interlok-profiler](https://github.com/adaptris/interlok-profiler) project; The class named TimedThroughputMetricMBean.

Metrics are generated for each of the following;
 - An Interlok [Consumer](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/AdaptrisMessageConsumer.html) consumes a message from your data-source such as a JMS queue, file-system, HTTP request etc.
 - A [Service](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/Service.html) processes a message, such as AddMetadataService, JdbcDataQueryService etc
 - A [Producer](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/AdaptrisMessageProducer.html) produces your message to your chosen endpoint such as JMS queue, file-system, HTTP response etc.
 - A [Workflow](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/Workflow.html) has finished processing a message from the Consumer, though all configured services all the way to the Producer.

The important methods for a [__TimedThroughputMetricMBean__](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-profiler/5.0-SNAPSHOT/com/adaptris/profiler/jmx/TimedThroughputMetricMBean.html) are;

| Method| Description |
|----|----|
| [getUniqueId()](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-profiler/4.8.0-RELEASE/com/adaptris/profiler/jmx/TimedThroughputMetricMBean.html#getUniqueId()--) | This field will return the components (consumer, producer or workflow) unique id. |
| [getMessageCount](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-profiler/4.8.0-RELEASE/com/adaptris/profiler/jmx/TimedThroughputMetricMBean.html#getMessageCount()--) | Will return the number of messages processed since the launch of the Interlok instance.
| [getWorkflowid](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-profiler/4.8.0-RELEASE/com/adaptris/profiler/jmx/TimedThroughputMetricMBean.html#getWorkflowId()--) | The id of the workflow that this component belongs to. |
| [getAverageNanoSeconds](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-profiler/4.8.0-RELEASE/com/adaptris/profiler/jmx/TimedThroughputMetricMBean.html#getAverageNanoseconds()--) | Will return the average time over the last 100 messages that this component takes to process a message |
| [getFailedMessageCount](https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-profiler/4.8.0-RELEASE/com/adaptris/profiler/jmx/TimedThroughputMetricMBean.html#getFailedMessageCount()--) | Simply the number of messages that have failed since the instance was launched. |


### Working with the metrics

You'll need to create your own Java project and make sure you have the interlok-profiler as a dependency and if you want to use the __JmxMBeanHelper__ as our example shows below you'll also need to include interlok-rest-base.  Assuming you're working with gradle and you've set-up the [Adaptris nexus](https://nexus.adaptris.net/nexus/content/groups/public) as a repository;

```
dependencies {
...
  implementation ("com.adaptris:interlok-profiler:5.0-RELEASE")
  implementation ("com.adaptris:interlok-rest-base:5.0-RELEASE")
}
```

Accessing the individual metrics for all components is relatively simple with the following code;
```java
private  static  final  String  PROFILER_OBJECT_NAME  =  "com.adaptris:type=Profiler,*";
...
// Query JMX to get a list of all metric objects.
Set<ObjectName> queryMBeans = JmxMBeanHelper().getMBeanNames(PROFILER_OBJECT_NAME);

// For each metric object...
queryMBeans.forEach(object -> {
    TimedThroughputMetricMBean  mBean = JmxMBeanHelper().proxyMBean(object, TimedThroughputMetricMBean.class);

    // If no workflow ID, then this may be an Interlok internal event or the base workflow rest HTTP acceptor service so simply ignore this one.
    if (mBean.getWorkflowId() != null)  {
        // Do something with the metric data
    }
});
```
