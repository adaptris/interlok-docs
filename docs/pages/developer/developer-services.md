# Writing your own Service

The [Service][] interface allows arbitrary functionality to be applied to [AdaptrisMessage][] objects in a [Workflow][]. It inherits some methods from other interfaces, namely [AdaptrisComponent][] and [StateManagedComponent][], but there are default implementations provided for those. There is only one key method in addition to [AdaptrisComponent]: this is the [doService()][] method which applies the appropriate action on the [AdaptrisMessage][] object.

[AdaptrisComponent][] defines methods common to all major components in the framework such as connections, consumers, producers and services. This is the interface that all components inherit. It primarily defines the component lifecycle methods for the framework. By having these methods we enforce a consistent state transition model within internally when the components are used.

[StateManagedComponent][] defines additional methods for enforcing transitions within the state. Rather than calling the `init()` method within code, you should make use of the various [LifecycleHelper][] methods which will enforce transitions correctly.

?> **TIP** An example quickstart project for services is available on github : [https://github.com/adaptris/interlok-custom-component-example](https://github.com/adaptris/interlok-custom-component-example)


## Minimum number of methods ##


If you simply extend [com.adaptris.core.ServiceImp][ServiceImp] then there are 3 methods that you must implement. They are [init()][], [close()][] and [doService(AdaptrisMessage)][doService()]. The only one that is of real interest is [doService(AdaptrisMessage)][doService()]. The others are inherited from [AdaptrisComponent][] and are related to managing the internal state of your service.

!> **IMPORTANT** If you make use of other [AdaptrisComponent] instances, then you should override all lifecycle methods [init()][], [start()][], [stop()][], [close()][] and make sure those instances are transitioned correctly.

## Full Example ##

Let's say that the `com.adaptris.whatever` package contains a class `DoSomething` that does something. It defines a constructor and two methods (for the sake of brevity we have skipped the actual implementations as they are not interesting to us).

```java
public DoSomething(String when, String how) {}
public void destroy() {}
public String doSomething(String theThing) throws Exception {}
```

The following class shows an implementation of Service that takes the result of the `doSomething(String)` method and applies that to the [AdaptrisMessage][] payload.

```java
package my.package.name;

import com.adaptris.whatever.*;
import com.adaptris.core.*;
import com.adaptris.core.util.*;
import com.thoughtworks.xstream.annotations.XStreamAlias;
import org.hibernate.validator.constraints.NotBlank;

@XStreamAlias("do-something-service")
public class DoSomethingService extends ServiceImp {

  @Getter
  @Setter
  @NotBlank
  private String how;
  @Getter
  @Setter
  @NotBlank
  private String when;
  private transient DoSomething doSomething;

  @Override
  protected void initService() throws CoreException {
    doSomething = new DoSomething(getWhen(), getHow());
  }

  @Override
  protected void closeService() {
    doSomething.destroy();
  }

  public void doService(AdaptrisMessage msg) throws ServiceException {
    try {
      String payload = msg.getContent();
      msg.setContentd(doSomething.doSomething(payload), msg.getContentEncoding());
    }
    catch(Exception e) {
      ExceptionHelper.rethrowServiceException(e);
    }
  }
}

```

So, the summary of what we did is as follows :

- We extended [com.adaptris.core.ServiceImp][ServiceImp] rather than implementing Service directly.
- The `initService()` method instantiates the class that provides the underlying functionality. This assumes that the class in question is fairly heavyweight and should not be re-created for each invocation of doService().
- The `closeService()` method calls `destroy()` on DoSomething to free resources.
- The start and stop methods are not required for this example. They are actually provided by ServiceImp as empty implementations.
- When catching and re-throwing Exceptions we use [ExceptionHelper][] to wrap the exception if it needs it; throwing the exception will cause error handling to be triggered.
- Public getter and setter methods are provided for the fields that are to be marshalled.

?> **TIP** The public getters/setters are not required by the marshaller, but will be required by the UI.


- The `DoSomething` member variable is marked as __transient__ so that XStream does not attempt to marshal it.
- `@NotBlank` annotations are added to the `how` and `when` member variables as validator hints for both the schema validator and UI that those fields need to be populated.
- An `@XStreamAlias` is added so that we have an alias that we can configure; so now, configuration is `<do-something-service>` rather than `<my.package.name.DoSomethingService>`


# Writing Tests #

Of course, you're going to be writing tests.  Add the following dependencies to your projects build.gradle;
```yaml
ext {
...
    junitVersion = '5.9.3'
    interlokCoreVersion = '5.0-SNAPSHOT'
}

dependencies {
...
    testImplementation ("org.junit.jupiter:junit-jupiter-api:$junitVersion")
    testImplementation ("org.junit.jupiter:junit-jupiter-engine:$junitVersion")
    testImplementation ("com.adaptris:interlok-stubs:$interlokCoreVersion") { changing= true }
}
```


As we are writing a [Service][] then you can add `com.adaptris:interlok-stubs` as a [dependency](/pages/developer/developer-compiling). This then means you can simply extend `com.adaptris.interlok.junit.scaffolding.services.ExampleServiceCase` and implement the required method `retrieveObjectForSampleConfig()`. Simply implementing that method automatically executes some tests for you provided by `ExampleServiceCase`:

- Automatic XML round trip testing; it will reflectively test that your service that has gone through the marshalling process is logically identical to one that was created programatically.
- Generate example XML; this requires that you have a `unit-test.properties` file available on the classpath for the tests.
    - In this file you need to have a property : `ServiceCase.baseDir` which is set to be a directory e.g. `ServiceCase.baseDir=./build/examples`.

So, based on our previous example, our test class could be something like

```java
package my.package.name;

import com.adaptris.core.AdaptrisMessageFactory;
import com.adaptris.core.ServiceException;
import com.adaptris.interlok.junit.scaffolding.services.ExampleServiceCase;

import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.fail;

@SuppressWarnings("deprecation")
public class DoSomethingTest extends ExampleServiceCase {

  public DoSomethingTest(java.lang.String testName) {
    super(testName);
  }

  @Test
  public void testService() throws Exception {
    try {
      execute(new DoSomethingService(), AdaptrisMessageFactory.getDefaultInstance().newMessage("Hello World"));
    } catch (Exception ex) {
      fail("Should not have failed for some reason.");
    }
  }

  @Override
  protected DoSomethingService retrieveObjectForSampleConfig() {
    DoSomethingService service = new DoSomethingService();
    service.setWhen("This is When");
    service.setHow("And This is How");
    return service;
  }

}

```

Post running the tests; we should have a file `./build/examples/my.package.name.DoSomethingService.xml` which contains (the unique-id is skipped in the example, but will be present):

```xml
<dummy-placeholder-service-element>
 <services>
  <do-something-service>
   <when>This is When<when>
   <how>And This Is How</how>
  </do-something-service>
 </services>
</dummy-placeholder-service-element>
```

There are similar classes that provide test scaffolding for other types of components.


[AdaptrisComponent]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/AdaptrisComponent.html
[Workflow]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/Workflow.html
[Service]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/Service.html
[StateManagedComponent]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/StateManagedComponent.html
[LifecycleHelper]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/util/LifecycleHelper.html
[ServiceImp]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/ServiceImp.html
[AdaptrisMessage]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/AdaptrisMessage.html
[ExceptionHelper]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/util/ExceptionHelper.html
[doService()]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/Service.html#doService-com.adaptris.core.AdaptrisMessage-
[init()]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/ComponentLifecycle.html#init--
[start()]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/ComponentLifecycle.html#start--
[stop()]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/ComponentLifecycle.html#stop--
[close()]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-core/5.0-SNAPSHOT/com/adaptris/core/ComponentLifecycle.html#close--
