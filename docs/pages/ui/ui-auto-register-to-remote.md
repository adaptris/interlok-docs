> **Summary:** This page explains how to auto register an adapter to remote UI Dashboard

When using multiple Interlok instances, maybe on different docker containers, it's sometimes better to monitor all of them with just one UI.

You can of course register them manually in the [UI Dashboard page](/pages/ui/ui-dashboard) or using the [UI REST API](/pages/developer/developer-ui-api).

However you may want the Interlok instances to register themselves so the UI is becomes aware of each instances only when they've started and registered.

## Registering an Interlok instance

In order to do that you can use the Interlok Exec (interlok-exec) optional component and a small bash script:

* First, i you need to install interlok-exec in the lib directory.

* Then, the bootstrap.properties need the following properties: 

```
...
managementComponents=jmx:jetty:exec
...
exec.registerinui.start.command=./bin/register-in-ui.sh
# 1 Year, we don't want to monitor this process
exec.registerinui.process.monitor.ms=31556952000
exec.registerinui.process.debug=true
...
```

* And finally, a bash script doing an http call to the [UI REST API](/pages/developer/developer-ui-api):

**register-in-ui.sh**

```
#!/bin/bash

```

```
#!/bin/bash

### Remote UI Details ###
REMOTE_UI_URL="http://localhost:8082/interlok/api/external/adapter"
REMOTE_UI_USER="admin"
# Base 64 encoded password (admin) but you may use environment properties
REMOTE_UI_PASSWORD="YWRtaW4="
REMOTE_UI_DECODED_PASSWORD=$(echo -ne "$REMOTE_UI_PASSWORD" | base64 -d)
REMOTE_UI_AUTH=$(echo -ne "$REMOTE_UI_USER:$REMOTE_UI_DECODED_PASSWORD" | base64 --wrap 0)

### This Adapter Details ###
# The JMX or Jolokia url that is accessible by the remote UI
TO_REGISTER_URL="service:jmx:jmxmp://localhost:5555"
TO_REGISTER_UID="MyInterlokInstance"
TO_REGISTER_NAME="MyInterlokInstance Jolokia"

### Curl command ###
echo "Excuting curl command to add adapter '$TO_REGISTER_NAME' to '$REMOTE_UI_URL'"
# Register the Adapter
curl -s -X POST $REMOTE_UI_URL -H  "accept: application/json" -H  "Content-Type: application/json" -H "Authorization: Basic $REMOTE_UI_AUTH" -d "{\"jmxUid\":\"$TO_REGISTER_UID\",\"url\":\"$TO_REGISTER_URL\",\"name\":\"$TO_REGISTER_NAME\"}"
```

If your Interlok instance is password protected you can add the username and password in the curl command payload:

```
curl -s -X POST $REMOTE_UI_URL -H  "accept: application/json" -H  "Content-Type: application/json" -H "Authorization: Basic $REMOTE_UI_AUTH" -d "{\"jmxUid\":\"$TO_REGISTER_UID\",\"url\":\"$TO_REGISTER_URL\",\"jmxUsername\":\"$TO_REGISTER_USER\",\"jmxPassword\":\"$TO_REGISTER_PASSWORD\",\"name\":\"$TO_REGISTER_NAME\"}"
```

## Registering and removing an Interlok instance

You may want to register an Interlok instance when it starts and remove it when it stop.

To do that you should follow the same principal as mentioned above but using the interlok-exec stop command as well.

```
...
managementComponents=jmx:jetty:exec
...
exec.registerinui.start.command=./bin/register-in-ui.sh register
exec.registerinui.stop.command=./bin/register-in-ui.sh remove
# 1 Year, we don't want to monitor this process
exec.registerinui.process.monitor.ms=31556952000
exec.registerinui.process.debug=true
...
```

You can also see that we provided arguments to our script, 'register' for the start command and 'remove' for the stop command.

We need to modify our script to deal with those arguments:

```
#!/bin/bash

ACTION=$1

### Remote UI Details ###
REMOTE_UI_URL="http://localhost:8082/interlok/api/external/adapter"
REMOTE_UI_USER="admin"
# Base 64 encoded password (admin) but you may use environment properties
REMOTE_UI_PASSWORD="YWRtaW4="
REMOTE_UI_DECODED_PASSWORD=$(echo -ne "$REMOTE_UI_PASSWORD" | base64 -d)
REMOTE_UI_AUTH=$(echo -ne "$REMOTE_UI_USER:$REMOTE_UI_DECODED_PASSWORD" | base64 --wrap 0)

### This Adapter Details ###
# The JMX or Jolokia url that is accessible by the remote UI
TO_REGISTER_URL="service:jmx:jmxmp://localhost:5555"
TO_REGISTER_UID="MyInterlokInstance"

function register()
{
  echo "Excuting curl command to add adapter '$TO_REGISTER_NAME' to '$REMOTE_UI_URL'"
  # Register the Adapter
  curl -s -X POST $REMOTE_UI_URL -H  "accept: application/json" -H  "Content-Type: application/json" -H "Authorization: Basic $REMOTE_UI_AUTH" -d "{\"jmxUid\":\"$TO_REGISTER_UID\",\"url\":\"$TO_REGISTER_URL\",\"name\":\"$TO_REGISTER_NAME\"}"
}

function remove()
{
  echo "Excuting curl command to remove adapter '$TO_REGISTER_NAME' from '$REMOTE_UI_URL'"
  # Remove the Adapter
  curl -s -X DELETE "$REMOTE_UI_URL/$TO_REGISTER_NAME" -H  "accept: application/json" -H "Authorization: Basic $REMOTE_UI_AUTH"
}

if [[ "$ACTION" = "register" ]]
then
  register
elif [[ "$ACTION" = "remove" ]]
then
  remove
else
  echo "'register' or 'remove' should be provided"
fi
```
