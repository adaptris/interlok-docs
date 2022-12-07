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

```xml
<?xml version="1.0"?>
<!DOCTYPE Configure PUBLIC "-//Jetty//Configure//EN" "http://www.eclipse.org/jetty/configure.dtd">
<!-- =============================================================== -->
<!-- Configure the Jetty Server                                      -->
<!-- Documentation of this file format can be found at:              -->
<!-- http://wiki.eclipse.org/Jetty/Reference/jetty.xml_syntax        -->
<!-- =============================================================== -->
<Configure id="Server" class="org.eclipse.jetty.server.Server">

  <New id="RewriteHandler" class="org.eclipse.jetty.rewrite.handler.RewriteHandler">
    <Set name="rewriteRequestURI">true</Set>
    <Set name="rewritePathInfo">false</Set>
    <Set name="originalPathAttribute">requestedPath</Set>
    <Call name="addRule">
      <Arg>
        <New class="org.eclipse.jetty.rewrite.handler.RedirectPatternRule">
          <Set name="pattern">/adapter-web-gui/*</Set>
          <Set name="location">/interlok</Set>
          <Set name="terminating">true</Set>
        </New>
      </Arg>
    </Call>
  </New>

  <Call id="MBeanServer" class="java.lang.management.ManagementFactory"
    name="getPlatformMBeanServer" />

  <Call name="addBean">
    <Arg>
      <New id="MBeanContainer" class="org.eclipse.jetty.jmx.MBeanContainer">
        <Arg>
          <Ref refid="MBeanServer" />
        </Arg>
      </New>
    </Arg>
  </Call>

  <Call name="addBean">
    <Arg>
      <New class="org.eclipse.jetty.util.log.Log" />
    </Arg>
  </Call>

  <Get name="ThreadPool">
     <Set name="minThreads" type="int">20</Set>
     <Set name="maxThreads" type="int">200</Set>
     <Set name="idleTimeout" type="int">60000</Set>
     <Set name="detailedDump">false</Set>
  </Get>

    <New id="httpConfig" class="org.eclipse.jetty.server.HttpConfiguration">
      <Set name="secureScheme"><Property name="jetty.httpConfig.secureScheme" default="https" /></Set>
      <Set name="securePort"><Property name="jetty.httpConfig.securePort" deprecated="jetty.secure.port" default="8443" /></Set>
      <Set name="outputBufferSize"><Property name="jetty.httpConfig.outputBufferSize" deprecated="jetty.output.buffer.size" default="32768" /></Set>
      <Set name="outputAggregationSize"><Property name="jetty.httpConfig.outputAggregationSize" deprecated="jetty.output.aggregation.size" default="8192" /></Set>
      <Set name="requestHeaderSize"><Property name="jetty.httpConfig.requestHeaderSize" deprecated="jetty.request.header.size" default="8192" /></Set>
      <Set name="responseHeaderSize"><Property name="jetty.httpConfig.responseHeaderSize" deprecated="jetty.response.header.size" default="8192" /></Set>
      <Set name="sendServerVersion"><Property name="jetty.httpConfig.sendServerVersion" deprecated="jetty.send.server.version" default="true" /></Set>
      <Set name="sendDateHeader"><Property name="jetty.httpConfig.sendDateHeader" deprecated="jetty.send.date.header" default="false" /></Set>
      <Set name="headerCacheSize"><Property name="jetty.httpConfig.headerCacheSize" default="512" /></Set>
      <Set name="delayDispatchUntilContent"><Property name="jetty.httpConfig.delayDispatchUntilContent" deprecated="jetty.delayDispatchUntilContent" default="true"/></Set>
      <Set name="maxErrorDispatches"><Property name="jetty.httpConfig.maxErrorDispatches" default="10"/></Set>
      <Set name="blockingTimeout"><Property name="jetty.httpConfig.blockingTimeout" default="-1"/></Set>
      <Set name="persistentConnectionsEnabled"><Property name="jetty.httpConfig.persistentConnectionsEnabled" default="true"/></Set>
    </New>

  <Call name="addConnector">
    <Arg>
      <New id="httpConnector" class="org.eclipse.jetty.server.ServerConnector">
        <Arg name="server"><Ref refid="Server" /></Arg>
        <Arg name="acceptors" type="int"><Property name="jetty.http.acceptors" deprecated="http.acceptors" default="-1"/></Arg>
        <Arg name="selectors" type="int"><Property name="jetty.http.selectors" deprecated="http.selectors" default="-1"/></Arg>
        <Arg name="factories">
          <Array type="org.eclipse.jetty.server.ConnectionFactory">
            <Item>
              <New class="org.eclipse.jetty.server.HttpConnectionFactory">
                <Arg name="config"><Ref refid="httpConfig" /></Arg>
                <Arg name="compliance"><Call class="org.eclipse.jetty.http.HttpCompliance" name="valueOf"><Arg><Property name="jetty.http.compliance" default="RFC7230"/></Arg></Call></Arg>
              </New>
            </Item>
          </Array>
        </Arg>
        <Set name="host"><Property name="jetty.http.host" deprecated="jetty.host" /></Set>
        <Set name="port"><Property name="jetty.http.port" deprecated="jetty.port" default="8080" /></Set>
        <Set name="idleTimeout"><Property name="jetty.http.idleTimeout" deprecated="http.timeout" default="30000"/></Set>
        <Set name="soLingerTime"><Property name="jetty.http.soLingerTime" deprecated="http.soLingerTime" default="-1"/></Set>
        <Set name="acceptorPriorityDelta"><Property name="jetty.http.acceptorPriorityDelta" deprecated="http.acceptorPriorityDelta" default="0"/></Set>
        <Set name="acceptQueueSize"><Property name="jetty.http.acceptQueueSize" deprecated="http.acceptQueueSize" default="0"/></Set>
      </New>
    </Arg>
  </Call>
  <Set name="handler">
    <New id="Handlers" class="org.eclipse.jetty.server.handler.HandlerList">
      <Set name="handlers">
        <Array type="org.eclipse.jetty.server.Handler">
          <Item>
            <Ref id="RewriteHandler"></Ref>
          </Item>
          <Item>
             <New id="Contexts" class="org.eclipse.jetty.server.handler.ContextHandlerCollection"/>
           </Item>
           <Item>
             <New id="DefaultHandler" class="org.eclipse.jetty.server.handler.DefaultHandler"/>
           </Item>
        </Array>
      </Set>
    </New>
  </Set>

  <Set name="stopAtShutdown">true</Set>
  <Set name="stopTimeout">1000</Set>
  <Set name="dumpAfterStart">false</Set>
  <Set name="dumpBeforeStop">false</Set>

  <Array id="plusConfig" type="java.lang.String">
    <Item>org.eclipse.jetty.webapp.WebInfConfiguration</Item>
    <Item>org.eclipse.jetty.webapp.WebXmlConfiguration</Item>
    <Item>org.eclipse.jetty.webapp.MetaInfConfiguration</Item>
    <Item>org.eclipse.jetty.webapp.FragmentConfiguration</Item>
    <Item>org.eclipse.jetty.plus.webapp.EnvConfiguration</Item>
    <Item>org.eclipse.jetty.plus.webapp.PlusConfiguration</Item>
    <Item>org.eclipse.jetty.webapp.JettyWebXmlConfiguration</Item>
  </Array>

  <Call name="addBean">
    <Arg>
      <New id="DeploymentManager" class="org.eclipse.jetty.deploy.DeploymentManager">
        <Set name="contexts">
          <Ref id="Contexts" />
        </Set>
        <Call name="setContextAttribute">
          <Arg>org.eclipse.jetty.server.webapp.ContainerIncludeJarPattern</Arg>
          <Arg>.*/[^/]*servlet-api-[^/]*\.jar$|.*/javax.servlet.jsp.jstl-.*\.jar$|.*/org.apache.taglibs.taglibs-standard-impl-.*\.jar$</Arg>
        </Call>
        <Call id="webappprovider" name="addAppProvider">
          <Arg>
            <New class="org.eclipse.jetty.deploy.providers.WebAppProvider">
              <Set name="monitoredDirName">
                <Property>
                  <Name>jetty.deploy.monitoredPath</Name>
                  <Default>
                    <Property name="jetty.base" default="." />/webapps
                  </Default>
                </Property>
              </Set>
              <Set name="defaultsDescriptor">
                <Property>
                  <Name>jetty.deploy.defaultsDescriptorPath</Name>
                  <Default>
                    <Property name="jetty.home" default="." />/config/webdefault.xml
                  </Default>
                </Property>
              </Set>
              <Set name="scanInterval"><Property name="jetty.deploy.scanInterval" default="120"/></Set>
              <Set name="extractWars"><Property name="jetty.deploy.extractWars" default="true"/></Set>
              <Set name="configurationClasses">
                <Ref id="plusConfig" />
              </Set>
              <Set name="configurationManager">
                <New class="org.eclipse.jetty.deploy.PropertiesConfigurationManager">
                </New>
              </Set>
            </New>
          </Arg>
        </Call>
      </New>
    </Arg>
  </Call>
</Configure>
```

Notice in the jetty.xml, there is a port defination:

```xml
<Set name="port"><Property name="jetty.http.port" deprecated="jetty.port" default="8080" /></Set>
```

If you wanted the UI to appear on port 8085, you would change this default="8080" to default="8085"

## webdefault.xml ##

As we are overriding the jetty.xml, we also need to provide a webdefault.xml

So, create a file called 'webdefault.xml' and also place this in the Interlok config folder.

Here is an example webdefault.xml:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app
   xmlns="http://xmlns.jcp.org/xml/ns/javaee"
   xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
   xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_3_1.xsd"
   metadata-complete="false"
   version="3.1">

  <description>
    Default web.xml file.
    This file is applied to a Web application before it's own WEB_INF/web.xml file
  </description>

  <listener>
   <listener-class>org.eclipse.jetty.servlet.listener.ELContextCleaner</listener-class>
  </listener>

  <listener>
   <listener-class>org.eclipse.jetty.servlet.listener.IntrospectorCleaner</listener-class>
  </listener>

  <servlet>
    <servlet-name>default</servlet-name>
    <servlet-class>org.eclipse.jetty.servlet.DefaultServlet</servlet-class>
    <init-param>
      <param-name>aliases</param-name>
      <param-value>false</param-value>
    </init-param>
    <init-param>
      <param-name>acceptRanges</param-name>
      <param-value>true</param-value>
    </init-param>
    <init-param>
      <param-name>dirAllowed</param-name>
      <param-value>true</param-value>
    </init-param>
    <init-param>
      <param-name>welcomeServlets</param-name>
      <param-value>false</param-value>
    </init-param>
    <init-param>
      <param-name>redirectWelcome</param-name>
      <param-value>false</param-value>
    </init-param>
    <init-param>
      <param-name>maxCacheSize</param-name>
      <param-value>256000000</param-value>
    </init-param>
    <init-param>
      <param-name>maxCachedFileSize</param-name>
      <param-value>200000000</param-value>
    </init-param>
    <init-param>
      <param-name>maxCachedFiles</param-name>
      <param-value>2048</param-value>
    </init-param>
    <init-param>
      <param-name>etags</param-name>
      <param-value>false</param-value>
    </init-param>
    <init-param>
      <param-name>useFileMappedBuffer</param-name>
      <param-value>true</param-value>
    </init-param>
    <load-on-startup>0</load-on-startup>
  </servlet>

  <servlet-mapping>
    <servlet-name>default</servlet-name>
    <url-pattern>/</url-pattern>
  </servlet-mapping>


  <servlet id="jsp">
    <servlet-name>jsp</servlet-name>
    <servlet-class>org.eclipse.jetty.jsp.JettyJspServlet</servlet-class>
    <init-param>
      <param-name>logVerbosityLevel</param-name>
      <param-value>DEBUG</param-value>
    </init-param>
    <init-param>
      <param-name>fork</param-name>
      <param-value>false</param-value>
    </init-param>
    <init-param>
      <param-name>xpoweredBy</param-name>
      <param-value>false</param-value>
    </init-param>
    <init-param>
      <param-name>compilerTargetVM</param-name>
      <param-value>1.7</param-value>
    </init-param>
    <init-param>
      <param-name>compilerSourceVM</param-name>
      <param-value>1.7</param-value>
    </init-param>
    <load-on-startup>0</load-on-startup>
  </servlet>

  <servlet-mapping>
    <servlet-name>jsp</servlet-name>
    <url-pattern>*.jsp</url-pattern>
    <url-pattern>*.jspf</url-pattern>
    <url-pattern>*.jspx</url-pattern>
    <url-pattern>*.xsp</url-pattern>
    <url-pattern>*.JSP</url-pattern>
    <url-pattern>*.JSPF</url-pattern>
    <url-pattern>*.JSPX</url-pattern>
    <url-pattern>*.XSP</url-pattern>
  </servlet-mapping>

  <session-config>
    <session-timeout>30</session-timeout>
  </session-config>

  <welcome-file-list>
    <welcome-file>index.html</welcome-file>
    <welcome-file>index.htm</welcome-file>
    <welcome-file>index.jsp</welcome-file>
  </welcome-file-list>

  <locale-encoding-mapping-list>
    <locale-encoding-mapping>
      <locale>ar</locale>
      <encoding>ISO-8859-6</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>be</locale>
      <encoding>ISO-8859-5</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>bg</locale>
      <encoding>ISO-8859-5</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>ca</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>cs</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>da</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>de</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>el</locale>
      <encoding>ISO-8859-7</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>en</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>es</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>et</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>fi</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>fr</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>hr</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>hu</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>is</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>it</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>iw</locale>
      <encoding>ISO-8859-8</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>ja</locale>
      <encoding>Shift_JIS</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>ko</locale>
      <encoding>EUC-KR</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>lt</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>lv</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>mk</locale>
      <encoding>ISO-8859-5</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>nl</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>no</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>pl</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>pt</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>ro</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>ru</locale>
      <encoding>ISO-8859-5</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>sh</locale>
      <encoding>ISO-8859-5</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>sk</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>sl</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>sq</locale>
      <encoding>ISO-8859-2</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>sr</locale>
      <encoding>ISO-8859-5</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>sv</locale>
      <encoding>ISO-8859-1</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>tr</locale>
      <encoding>ISO-8859-9</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>uk</locale>
      <encoding>ISO-8859-5</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>zh</locale>
      <encoding>GB2312</encoding>
    </locale-encoding-mapping>
    <locale-encoding-mapping>
      <locale>zh_TW</locale>
      <encoding>Big5</encoding>
    </locale-encoding-mapping>
  </locale-encoding-mapping-list>

  <security-constraint>
    <web-resource-collection>
      <web-resource-name>Disable TRACE</web-resource-name>
      <url-pattern>/</url-pattern>
      <http-method>TRACE</http-method>
    </web-resource-collection>
    <auth-constraint/>
  </security-constraint>
  <security-constraint>
    <web-resource-collection>
      <web-resource-name>Enable everything but TRACE</web-resource-name>
      <url-pattern>/</url-pattern>
      <http-method-omission>TRACE</http-method-omission>
    </web-resource-collection>
  </security-constraint>

</web-app>

```

## bootstrap.properties ##

Finally, we need to update the bootstrap.properties (found in the config folder of Interlok)

We would need the following setting:


```properties
webServerConfigUrl=./config/jetty.xml
```

Now, if we have done all of the above, after an Interlok restart, the UI should be available at the new port.
