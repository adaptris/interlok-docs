# Accessing External Webservices

> **Summary:** This document is aimed at developers and system administrators who wish to make use to make calls to web-services outside of the domain of Interlok. Depending on how you want to execute the webservice; it will depend on interlok-webservice-cxf.

Adding this component to your Interlok installation will depend on the method used to build your installation, however gradle is the most common therefore simply add the following to your gradle dependencies list:

```
ext {
  ...
  interlokVersion='5.0-RELEASE'
}
...

dependencies {
  ...
  interlokRuntime ("com.adaptris:interlok-webservice-cxf:$interlokVersion") { changing=true }
}
```

To access an external webservice from Interlok simply use the [apache-cxf-soap-service][] which calls the webservice with the payload of the current message as the operation argument (the service will look after any required SOAP headers).


## Using apache-cxf-soap-service ##

You will need to know the structure of the webservice document (which can be easily discovered by using SoapUI against the WSDL); map to it, and configure the service appropriately. In the majority of cases, this is the only service you will need.

An important note:  You will be responsible for wrapping your intended payload with a SOAP wrapper; example below.

### Example ###

If we wanted to call a number converter webservice hosted by [dataaccess][www.dataaccess.com]; then we can do that quite easily using [apache-cxf-soap-service][]. For the purposes of our example we are going to provide a number (12) and have the number converter service return us the number in words.

In a single workflow, we'll add a polling trigger consumer that will execute the payload every 1 minute.

```xml
		  <consumer class="polling-trigger">
            <unique-id>admiring-gates</unique-id>
            <poller class="fixed-interval-poller">
              <poll-interval>
                <unit>MINUTES</unit>
                <interval>1</interval>
              </poll-interval>
            </poller>
            <message-provider class="static-polling-trigger-template">
              <template><![CDATA[
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <NumberToWords xmlns="http://www.dataaccess.com/webservicesserver/">
      <ubiNum>12</ubiNum>
    </NumberToWords>
  </soap:Body>
</soap:Envelope>
]]>
			  </template>
            </message-provider>
          </consumer>
```

Notice the payload contains the SOAP wrapping and specifically for this webservice we need to provide a number value in the *ubiNum* element.

Now we include our webservice client caller service;

```xml
              <apache-cxf-soap-service>
                <unique-id>number-converter-service</unique-id>
                <wsdl-url>https://www.dataaccess.com/webservicesserver/NumberConversion.wso?WSDL</wsdl-url>
                <port-name>NumberConversionSoap</port-name>
                <service-name>NumberConversion</service-name>
                <namespace>http://www.dataaccess.com/webservicesserver/</namespace>
              </apache-cxf-soap-service>
```

Executing this workflow will produce a payload like this;

```xml
<?xml version="1.0" encoding="UTF-8"?>
<m:NumberToWordsResponse xmlns:m="http://www.dataaccess.com/webservicesserver/">
  <m:NumberToWordsResult>twelve </m:NumberToWordsResult>
</m:NumberToWordsResponse>]
```


[apache-cxf-soap-service]: https://nexus.adaptris.net/nexus/content/sites/javadocs/com/adaptris/interlok-webservice-cxf/5.0-SNAPSHOT/com/adaptris/core/services/cxf/ApacheSoapService.html
[snapshot]: https://nexus.adaptris.net/nexus/content/groups/adaptris-snapshots/com/adaptris/interlok-webservice-external/
[release]: https://nexus.adaptris.net/nexus/content/groups/public/com/adaptris/interlok-webservice-external/