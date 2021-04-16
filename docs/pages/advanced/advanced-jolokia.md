# Jolokia Monitoring and Management (4.0.0+)

> **Summary:** The adapter supports monitoring over Jolokia protocol (JMX call via HTTP). This allows developers and administrators to manage and monitor the adapter via any HTTP client. By default, the adapter exposes a Jolokia endpoint on port `8081` with the context path `/jolokia` (`http://localhost:8081/jolokia/`), if the jolokia management component is enabled and interlok-jolokia is in the lib directory; this is configurable via some settings in your bootstrap.properties

## Port and Context Path ##

If the default port `8081` and the context path `/jolokia` are not your thing you can change then in bootstrap.properties

| Property | Description |
|----|----|
| jolokiaPort  | 8081
| jolokiaContextPath | /jolokia

## Password Protecting ##

By default there is no authentication of client connections to the default HTTP port. Password protection can be enabled through a couple of additional properties in bootstrap.properties which will enable a handler which verifies the supplied username and password combination.

| Property | Description |
|----|----|
| jolokiaUsername | The username
| jolokiaPassword | The password which may be encoded using the [password handling mechanism](/pages/advanced/advanced-password-handling).|

## Example ##

Using your favourite HTTP GET/POST tool, make a POST request to the running Interlok Jolokia instance at http://localhost:8081/jolokia/:

### Read ###
Request

```
curl --location --request POST 'http://localhost:8081/jolokia/' --header 'Content-Type: application/json' --header 'Accept: application/json' \
--data-raw '{
  "type" : "READ",
  "mbean" : "com.adaptris:type=Adapter,id=MyInterlokInstance",
  "attribute": "ComponentState"
}'
```

Response

```
{
  "request": {
    "mbean": "com.adaptris:id=MyInterlokInstance,type=Adapter",
    "attribute": "ComponentState",
    "type": "read"
  },
  "value": "StartedState",
  "timestamp": 1612416801,
  "status": 200
}

```
### Exec ###

Request

```
curl --location --request POST 'http://localhost:8081/jolokia/' --header 'Content-Type: application/json' --header 'Accept: application/json' \
--data-raw '{
  "type" : "EXEC",
  "mbean" : "com.adaptris:type=Adapter,id=MyInterlokInstance",
  "operation": "requestStart()"
}'
```

Response

```
{
  "request": {
    "mbean": "com.adaptris:id=MyInterlokInstance,type=Adapter",
    "type": "exec",
    "operation": "requestStart()"
  },
  "value": null,
  "timestamp": 1612416801,
  "status": 200
}
```

### Search ###

Request

```
curl --location --request POST 'http://localhost:8081/jolokia/' --header 'Content-Type: application/json' --header 'Accept: application/json' \
--data-raw '{
  "type" : "SEARCH",
  "mbean" : "com.adaptris:type=Workflow,adapter=MyInterlokInstance,channel=*,id=*"
}'
```

Response

```
{
  "request": {
    "mbean": "com.adaptris:adapter=MyInterlokInstance,channel=*,id=*,type=Workflow",
    "type": "search"
  },
  "value": [
    "com.adaptris:adapter=MyInterlokInstance,channel=Channel1,id=Workflow11,type=Workflow",
    "com.adaptris:adapter=MyInterlokInstance,channel=Channel1,id=Workflow12,type=Workflow",
    "com.adaptris:adapter=MyInterlokInstance,channel=Channel2,id=Workflow21,type=Workflow",
    "com.adaptris:adapter=MyInterlokInstance,channel=Channel2,id=Workflow22,type=Workflow",
    "com.adaptris:adapter=MyInterlokInstance,channel=Channel3,id=Workflow31,type=Workflow",
    "com.adaptris:adapter=MyInterlokInstance,channel=Channel3,id=Workflow33,type=Workflow"
  ],
  "timestamp": 1612419632,
  "status": 200
}
```

## More ##

You can read more about jolokia protocol at https://jolokia.org/reference/html/protocol.html#post-request

GET request can also be used for simple queries (https://jolokia.org/reference/html/protocol.html#get-request) but Jolokia recommend to use POST requests.
