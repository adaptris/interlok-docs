By default the Interlok UI is reachable on port 8080, http://localhost:8080/interlok/

If you wish to change the port number, you have to configure Interloks embedded jetty engine.

The following steps are required:

- Configure a 'jetty.xml'
- Configure a 'webdefault.xml'
- Configure the 'bootstrap.properties' to use your jetty.xml

There is a lot more you can do in the jetty configuration than just change the port number, but that's all we are going to talk about in this page.

## jetty.xml ##

First, create a file called 'jetty.xml' and place this in the Interlok config folder.

Here is an example jetty.xml:

[jetty.xml](https://raw.githubusercontent.com/adaptris/interlok/master/interlok-common/src/main/resources/com/adaptris/core/management/webserver/jetty-failsafe.xml ':include :type=code')

Notice in the jetty.xml, there is a port definition:

```xml
<Set name="port"><Property name="jetty.http.port" deprecated="jetty.port" default="8080" /></Set>
```

If you wanted the UI to appear on port 8085, you would change this default="8080" to default="8085"

## webdefault.xml ##

As we are overriding the jetty.xml, we also need to provide a webdefault.xml

So, create a file called 'webdefault.xml' and also place this in the Interlok config folder.

Here is an example webdefault.xml:

[webdefault.xml](https://raw.githubusercontent.com/adaptris/interlok/master/interlok-common/src/main/resources/com/adaptris/core/management/webserver/jetty-webdefault-failsafe.xml ':include :type=code')

## bootstrap.properties ##

Finally, we need to update the bootstrap.properties (found in the config folder of Interlok)

We would need the following setting:


```properties
webServerConfigUrl=./config/jetty.xml
```

Now, if we have done all of the above, after an Interlok restart, the UI should be available at the new port.
