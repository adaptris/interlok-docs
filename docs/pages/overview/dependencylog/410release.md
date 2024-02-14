## Version 4.1.0 ##

### interlok-activemq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- org.apache.activemq:activemq-amqp:5.16.2
- org.apache.activemq:activemq-broker:5.16.2
- org.apache.activemq:activemq-client:5.16.2
- org.apache.activemq:activemq-jaas:5.16.2
- org.apache.activemq:activemq-kahadb-store:5.16.2
- org.apache.activemq:activemq-mqtt:5.16.2
- org.apache.activemq:activemq-spring:5.16.2
- org.apache.activemq:activemq-stomp:5.16.2
- org.springframework:spring-beans:5.3.7
- org.springframework:spring-context:5.3.7

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- org.apache.activemq:activemq-amqp:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-broker:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-client:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-jaas:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-kahadb-store:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-mqtt:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-spring:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-stomp:5.16.2 *(from 5.16.1)*
- org.springframework:spring-beans:5.3.7 *(from 5.3.4)*
- org.springframework:spring-context:5.3.7 *(from 5.3.4)*

### interlok-amqp ###

#### New Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:2.3.0
- com.rabbitmq:amqp-client:5.12.0
- io.netty:netty-buffer:4.1.65.Final
- io.netty:netty-codec-http:4.1.65.Final
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-common:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final
- io.netty:netty-transport-native-kqueue:4.1.65.Final
- io.netty:netty-transport-native-unix-common:4.1.65.Final
- io.netty:netty-transport:4.1.65.Final
- org.apache.qpid:qpid-jms-client:1.0.0

#### Updated Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:2.3.0 *(from 2.2.0)*
- com.rabbitmq:amqp-client:5.12.0 *(from 5.11.0)*
- io.netty:netty-buffer:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec-http:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-common:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-handler:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-epoll:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-kqueue:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-unix-common:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport:4.1.65.Final *(from 4.1.60.Final)*
- org.apache.qpid:qpid-jms-client:1.0.0 *(from 0.56.0)*

### interlok-apache-geode ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- commons-codec:commons-codec:1.15
- org.apache.geode:geode-core:1.13.2

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- org.apache.geode:geode-core:1.13.2 *(from 1.13.1)*

### interlok-apache-http ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.30

#### Removed Dependencies ####
- ~~commons-codec:commons-codec:1.15~~
- ~~org.apache.commons:commons-lang3:3.12.0~~

### interlok-apache-http5 ###

#### Initial Dependencies ####
- org.apache.httpcomponents.client5:httpclient5:5.1
- org.slf4j:slf4j-api:1.7.30

### interlok-artemis ###

#### New Dependencies ####
- io.netty:netty-buffer:4.1.65.Final
- io.netty:netty-codec-http:4.1.65.Final
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-common:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final
- io.netty:netty-transport-native-kqueue:4.1.65.Final
- io.netty:netty-transport-native-unix-common:4.1.65.Final
- io.netty:netty-transport:4.1.65.Final

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec-http:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-common:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-handler:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-epoll:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-kqueue:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-unix-common:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport:4.1.65.Final *(from 4.1.60.Final)*

### interlok-aws-common ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.amazonaws:aws-java-sdk-sts:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034 *(from 1.11.974)*
- com.amazonaws:aws-java-sdk-sts:1.11.1034 *(from 1.11.974)*
- com.fasterxml.jackson.core:jackson-annotations:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3 *(from 2.12.2)*

### interlok-aws-kinesis ###

#### New Dependencies ####
- com.amazonaws:amazon-kinesis-client:1.14.3
- com.amazonaws:amazon-kinesis-producer:0.14.7
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.amazonaws:aws-java-sdk-kinesis:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3
- com.google.guava:guava:30.1.1-jre
- com.google.protobuf:protobuf-java:3.17.2
- io.netty:netty-buffer:4.1.65.Final
- io.netty:netty-codec-http:4.1.65.Final
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-common:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final
- io.netty:netty-transport-native-kqueue:4.1.65.Final
- io.netty:netty-transport-native-unix-common:4.1.65.Final
- io.netty:netty-transport:4.1.65.Final

#### Updated Dependencies ####
- com.amazonaws:amazon-kinesis-client:1.14.3 *(from 1.14.2)*
- com.amazonaws:amazon-kinesis-producer:0.14.7 *(from 0.14.6)*
- com.amazonaws:aws-java-sdk-kinesis:1.11.1034 *(from 1.11.974)*
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.google.protobuf:protobuf-java:3.17.2 *(from 3.15.6)*

### interlok-aws-kinesis-sdk ###

#### Initial Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.amazonaws:aws-java-sdk-kinesis:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3
- org.slf4j:jcl-over-slf4j:1.7.30
- org.slf4j:slf4j-api:1.7.30

### interlok-aws-kms ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.amazonaws:aws-java-sdk-kms:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-kms:1.11.1034 *(from 1.11.974)*

### interlok-aws-s3 ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.amazonaws:aws-java-sdk-s3:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.1034 *(from 1.11.974)*

### interlok-aws-sns ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.amazonaws:aws-java-sdk-sns:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.1034 *(from 1.11.974)*

### interlok-aws-sqs ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.amazonaws:aws-java-sdk-sqs:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sqs:1.11.1034 *(from 1.11.974)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*

### interlok-azure-core ###

#### New Dependencies ####
- com.azure:azure-identity:1.2.5
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-xml:2.12.3
- com.fasterxml.jackson.datatype:jackson-datatype-jsr310:2.12.3
- com.microsoft.azure:msal4j:1.10.0
- io.netty:netty-codec-http2:4.1.65.Final
- io.netty:netty-codec-http:4.1.65.Final
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-handler-proxy:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final
- io.netty:netty-transport-native-kqueue:4.1.65.Final
- io.netty:netty-transport-native-unix-common:4.1.65.Final
- net.minidev:json-smart:2.3.1

#### Updated Dependencies ####
- com.azure:azure-identity:1.2.5 *(from 1.2.1)*
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.dataformat:jackson-dataformat-xml:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.datatype:jackson-datatype-jsr310:2.12.3 *(from 2.12.2)*
- com.microsoft.azure:msal4j:1.10.0 *(from 1.8.1)*
- io.netty:netty-codec-http2:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec-http:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-handler-proxy:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-handler:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-epoll:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-kqueue:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-unix-common:4.1.65.Final *(from 4.1.60.Final)*

### interlok-azure-cosmosdb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.microsoft.azure:azure-documentdb:2.6.3

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.microsoft.azure:azure-documentdb:2.6.3 *(from 2.6.1)*

### interlok-cassandra ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- io.netty:netty-codec:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-handler:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-epoll:4.1.65.Final *(from 4.1.60.Final)*

### interlok-client ###

#### New Dependencies ####
- org.mockito:mockito-core:3.11.1
- org.mockito:mockito-inline:3.11.1

#### Updated Dependencies ####
- org.mockito:mockito-core:3.11.1 *(from 3.8.0)*
- org.mockito:mockito-inline:3.11.1 *(from 3.8.0)*

### interlok-client-jmx ###

#### New Dependencies ####
- org.mockito:mockito-core:3.11.1
- org.mockito:mockito-inline:3.11.1

#### Updated Dependencies ####
- org.mockito:mockito-core:3.11.1 *(from 3.8.0)*
- org.mockito:mockito-inline:3.11.1 *(from 3.8.0)*

### interlok-common ###

#### New Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- commons-io:commons-io:2.10.0
- org.apache.commons:commons-pool2:2.10.0
- org.eclipse.jetty.aggregate:jetty-all:9.4.42.v20210604
- org.mockito:mockito-core:3.11.1
- org.mockito:mockito-inline:3.11.1

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*
- commons-io:commons-io:2.10.0 *(from 2.8.0)*
- org.apache.commons:commons-pool2:2.10.0 *(from 2.9.0)*
- org.eclipse.jetty.aggregate:jetty-all:9.4.42.v20210604 *(from 9.4.39.v20210325)*
- org.mockito:mockito-core:3.11.1 *(from 3.8.0)*
- org.mockito:mockito-inline:3.11.1 *(from 3.8.0)*

### interlok-core ###

#### New Dependencies ####
- com.github.mwiede:jsch:0.1.63
- com.sun.mail:jakarta.mail:1.6.7
- com.thoughtworks.xstream:xstream:1.4.17
- commons-io:commons-io:2.10.0
- mysql:mysql-connector-java:8.0.25
- net.sf.saxon:Saxon-HE:10.5
- org.apache.activemq:activemq-broker:5.16.2
- org.apache.activemq:activemq-client:5.16.2
- org.apache.activemq:activemq-jaas:5.16.2
- org.apache.activemq:activemq-kahadb-store:5.16.2
- org.apache.commons:commons-pool2:2.10.0
- org.awaitility:awaitility:4.1.0
- org.bouncycastle:bcmail-jdk15on:1.69
- org.bouncycastle:bcpkix-jdk15on:1.69
- org.bouncycastle:bcprov-jdk15on:1.69
- org.eclipse.jetty.aggregate:jetty-all:9.4.42.v20210604
- org.jruby:jruby-complete:9.2.18.0
- org.mockito:mockito-core:3.11.1
- org.mockito:mockito-inline:3.11.1

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.1.63 *(from 0.1.62)*
- com.sun.mail:jakarta.mail:1.6.7 *(from 1.6.5)*
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*
- commons-io:commons-io:2.10.0 *(from 2.8.0)*
- mysql:mysql-connector-java:8.0.25 *(from 8.0.23)*
- net.sf.saxon:Saxon-HE:10.5 *(from 10.3)*
- org.apache.activemq:activemq-broker:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-client:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-jaas:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-kahadb-store:5.16.2 *(from 5.16.1)*
- org.apache.commons:commons-pool2:2.10.0 *(from 2.9.0)*
- org.awaitility:awaitility:4.1.0 *(from 4.0.3)*
- org.bouncycastle:bcmail-jdk15on:1.69 *(from 1.68)*
- org.bouncycastle:bcpkix-jdk15on:1.69 *(from 1.68)*
- org.bouncycastle:bcprov-jdk15on:1.69 *(from 1.68)*
- org.eclipse.jetty.aggregate:jetty-all:9.4.42.v20210604 *(from 9.4.39.v20210325)*
- org.jruby:jruby-complete:9.2.18.0 *(from 9.2.16.0)*
- org.mockito:mockito-core:3.11.1 *(from 3.8.0)*
- org.mockito:mockito-inline:3.11.1 *(from 3.8.0)*

### interlok-core-apt ###

#### New Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*

### interlok-csv-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*

### interlok-ehcache ###

#### New Dependencies ####
- net.sf.ehcache:ehcache:2.10.9.2

#### Updated Dependencies ####
- net.sf.ehcache:ehcache:2.10.9.2 *(from 2.10.6)*

### interlok-elastic-common ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.jayway.jsonpath:json-path:2.6.0
- net.sf.supercsv:super-csv:2.4.0

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.jayway.jsonpath:json-path:2.6.0 *(from 2.4.0)*

### interlok-elastic-rest ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.jayway.jsonpath:json-path:2.6.0

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.jayway.jsonpath:json-path:2.6.0 *(from 2.4.0)*

### interlok-filesystem ###

#### New Dependencies ####
- com.hierynomus:smbj:0.11.1
- org.apache.tika:tika-core:1.26

#### Updated Dependencies ####
- com.hierynomus:smbj:0.11.1 *(from 0.10.0)*
- org.apache.tika:tika-core:1.26 *(from 1.25)*

### interlok-flyway ###

#### New Dependencies ####
- org.flywaydb:flyway-core:7.9.2

#### Updated Dependencies ####
- org.flywaydb:flyway-core:7.9.2 *(from 7.7.0)*

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.google.cloud:google-cloud-pubsub:1.112.5
- com.google.code.gson:gson:2.8.7
- com.google.protobuf:protobuf-java-util:3.17.2
- com.google.protobuf:protobuf-java:3.17.2
- io.grpc:grpc-alts:1.38.0
- io.grpc:grpc-auth:1.38.0
- io.grpc:grpc-netty:1.38.0
- io.grpc:grpc-protobuf:1.38.0
- io.grpc:grpc-stub:1.38.0
- io.netty:netty-codec-http2:4.1.65.Final
- io.netty:netty-codec-http:4.1.65.Final
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.google.cloud:google-cloud-pubsub:1.112.5 *(from 1.111.4)*
- com.google.code.gson:gson:2.8.7 *(from 2.8.6)*
- com.google.protobuf:protobuf-java-util:3.17.2 *(from 3.15.6)*
- com.google.protobuf:protobuf-java:3.17.2 *(from 3.15.6)*
- io.grpc:grpc-alts:1.38.0 *(from 1.35.0)*
- io.grpc:grpc-auth:1.38.0 *(from 1.35.0)*
- io.grpc:grpc-netty:1.38.0 *(from 1.35.0)*
- io.grpc:grpc-protobuf:1.38.0 *(from 1.35.0)*
- io.grpc:grpc-stub:1.38.0 *(from 1.35.0)*
- io.netty:netty-codec-http2:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec-http:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-handler:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-epoll:4.1.65.Final *(from 4.1.60.Final)*

### interlok-jdbc ###

#### Initial Dependencies ####
- com.google.guava:guava:30.1.1-jre
- commons-codec:commons-codec:1.15
- org.codehaus.staxmate:stax2:2.1
- org.slf4j:slf4j-api:1.7.30

### interlok-jmx-activemq ###

#### New Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- org.apache.activemq:activemq-client:5.16.2
- org.springframework:spring-aop:5.3.7
- org.springframework:spring-beans:5.3.7
- org.springframework:spring-context:5.3.7
- org.springframework:spring-core:5.3.7
- org.springframework:spring-jms:5.3.7

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*
- org.apache.activemq:activemq-client:5.16.2 *(from 5.16.1)*
- org.springframework:spring-aop:5.3.7 *(from 5.3.5)*
- org.springframework:spring-beans:5.3.7 *(from 5.3.5)*
- org.springframework:spring-context:5.3.7 *(from 5.3.5)*
- org.springframework:spring-core:5.3.7 *(from 5.3.5)*
- org.springframework:spring-jms:5.3.7 *(from 5.3.5)*

### interlok-jmx-amqp ###

#### New Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- io.netty:netty-buffer:4.1.65.Final
- io.netty:netty-codec-http:4.1.65.Final
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-common:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final
- io.netty:netty-transport-native-kqueue:4.1.65.Final
- io.netty:netty-transport-native-unix-common:4.1.65.Final
- io.netty:netty-transport:4.1.65.Final
- org.apache.qpid:qpid-jms-client:1.0.0
- org.springframework:spring-aop:5.3.7
- org.springframework:spring-beans:5.3.7
- org.springframework:spring-context:5.3.7
- org.springframework:spring-core:5.3.7
- org.springframework:spring-jms:5.3.7

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*
- io.netty:netty-buffer:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec-http:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-codec:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-common:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-handler:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-epoll:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-kqueue:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-unix-common:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport:4.1.65.Final *(from 4.1.60.Final)*
- org.apache.qpid:qpid-jms-client:1.0.0 *(from 0.56.0)*
- org.springframework:spring-aop:5.3.7 *(from 5.3.5)*
- org.springframework:spring-beans:5.3.7 *(from 5.3.5)*
- org.springframework:spring-context:5.3.7 *(from 5.3.5)*
- org.springframework:spring-core:5.3.7 *(from 5.3.5)*
- org.springframework:spring-jms:5.3.7 *(from 5.3.5)*

### interlok-jmx-jms-common ###

#### New Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- org.springframework:spring-aop:5.3.7
- org.springframework:spring-beans:5.3.7
- org.springframework:spring-context:5.3.7
- org.springframework:spring-core:5.3.7
- org.springframework:spring-jms:5.3.7

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*
- org.springframework:spring-aop:5.3.7 *(from 5.3.5)*
- org.springframework:spring-beans:5.3.7 *(from 5.3.5)*
- org.springframework:spring-context:5.3.7 *(from 5.3.5)*
- org.springframework:spring-core:5.3.7 *(from 5.3.5)*
- org.springframework:spring-jms:5.3.7 *(from 5.3.5)*

### interlok-jmx-jms-stubs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.thoughtworks.xstream:xstream:1.4.17
- commons-io:commons-io:2.10.0
- org.apache.activemq:activemq-amqp:5.16.2
- org.apache.activemq:activemq-broker:5.16.2
- org.apache.activemq:activemq-jaas:5.16.2
- org.apache.activemq:activemq-kahadb-store:5.16.2
- org.springframework:spring-aop:5.3.7
- org.springframework:spring-beans:5.3.7
- org.springframework:spring-context:5.3.7
- org.springframework:spring-core:5.3.7
- org.springframework:spring-jms:5.3.7

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*
- commons-io:commons-io:2.10.0 *(from 2.8.0)*
- org.apache.activemq:activemq-amqp:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-broker:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-jaas:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-kahadb-store:5.16.2 *(from 5.16.1)*
- org.springframework:spring-aop:5.3.7 *(from 5.3.5)*
- org.springframework:spring-beans:5.3.7 *(from 5.3.5)*
- org.springframework:spring-context:5.3.7 *(from 5.3.5)*
- org.springframework:spring-core:5.3.7 *(from 5.3.5)*
- org.springframework:spring-jms:5.3.7 *(from 5.3.5)*

### interlok-jmx-solace ###

#### New Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- org.springframework:spring-aop:5.3.7
- org.springframework:spring-beans:5.3.7
- org.springframework:spring-context:5.3.7
- org.springframework:spring-core:5.3.7
- org.springframework:spring-jms:5.3.7

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*
- org.springframework:spring-aop:5.3.7 *(from 5.3.5)*
- org.springframework:spring-beans:5.3.7 *(from 5.3.5)*
- org.springframework:spring-context:5.3.7 *(from 5.3.5)*
- org.springframework:spring-core:5.3.7 *(from 5.3.5)*
- org.springframework:spring-jms:5.3.7 *(from 5.3.5)*

### interlok-jq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*

### interlok-jruby ###

#### New Dependencies ####
- org.jruby:jruby:9.2.17.0

#### Updated Dependencies ####
- org.jruby:jruby:9.2.17.0 *(from 9.2.16.0)*

### interlok-jslt ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*

### interlok-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.12.3
- com.github.everit-org.json-schema:org.everit.json.schema:1.12.2
- com.jayway.jsonpath:json-path:2.6.0
- xom:xom:1.3.7

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.12.3 *(from 2.12.2)*
- com.github.everit-org.json-schema:org.everit.json.schema:1.12.2 *(from 1.12.0)*
- com.jayway.jsonpath:json-path:2.6.0 *(from 2.4.0)*
- xom:xom:1.3.7 *(from 1.3.6)*

### interlok-json-streaming ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.github.jsurfer:jsurfer-gson:1.6.0
- com.github.jsurfer:jsurfer-jackson:1.6.0
- com.github.jsurfer:jsurfer-jsonsimple:1.6.0

### interlok-json-web-token ###

#### New Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.69
- org.bouncycastle:bcprov-jdk15on:1.69

#### Updated Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.69 *(from 1.68)*
- org.bouncycastle:bcprov-jdk15on:1.69 *(from 1.68)*

### interlok-kafka ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- io.netty:netty-codec:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-handler:4.1.65.Final *(from 4.1.60.Final)*
- io.netty:netty-transport-native-epoll:4.1.65.Final *(from 4.1.60.Final)*

### interlok-kie ###

#### New Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- org.drools:drools-compiler:7.54.0.Final
- org.drools:drools-core:7.54.0.Final

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*
- org.drools:drools-compiler:7.54.0.Final *(from 7.51.0.Final)*
- org.drools:drools-core:7.54.0.Final *(from 7.51.0.Final)*

### interlok-mail ###

#### New Dependencies ####
- com.sun.mail:jakarta.mail:1.6.7

#### Updated Dependencies ####
- com.sun.mail:jakarta.mail:1.6.7 *(from 1.6.5)*

### interlok-mongodb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*

### interlok-nats ###

#### New Dependencies ####
- io.nats:jnats:2.11.4

#### Updated Dependencies ####
- io.nats:jnats:2.11.4 *(from 2.8.0)*

### interlok-oauth-azure ###

#### New Dependencies ####
- com.microsoft.azure:adal4j:1.6.7
- net.minidev:json-smart:2.4.7

#### Updated Dependencies ####
- com.microsoft.azure:adal4j:1.6.7 *(from 1.6.6)*
- net.minidev:json-smart:2.4.7 *(from 2.3)*

### interlok-oauth-gcloud ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.google.auth:google-auth-library-oauth2-http:0.26.0

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.google.auth:google-auth-library-oauth2-http:0.26.0 *(from 0.24.1)*

### interlok-oauth-generic ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.jayway.jsonpath:json-path:2.6.0

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.jayway.jsonpath:json-path:2.6.0 *(from 2.4.0)*

### interlok-oauth-salesforce ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*

### interlok-pdf ###

#### New Dependencies ####
- commons-io:commons-io:2.10.0
- org.apache.pdfbox:fontbox:2.0.24
- org.apache.pdfbox:pdfbox-tools:2.0.24
- org.apache.pdfbox:pdfbox:2.0.24

#### Updated Dependencies ####
- org.apache.pdfbox:fontbox:2.0.24 *(from 2.0.23)*
- org.apache.pdfbox:pdfbox-tools:2.0.24 *(from 2.0.23)*
- org.apache.pdfbox:pdfbox:2.0.24 *(from 2.0.23)*

### interlok-pgp ###

#### New Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.69
- org.bouncycastle:bcprov-jdk15on:1.69

#### Updated Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.69 *(from 1.68)*
- org.bouncycastle:bcprov-jdk15on:1.69 *(from 1.68)*

### interlok-profiler ###

#### New Dependencies ####
- org.apache.commons:commons-math3:3.6.1

### interlok-rest-metrics-jvm ###

#### New Dependencies ####
- io.micrometer:micrometer-core:1.7.0

#### Removed Dependencies ####
- ~~io.micrometer:micrometer-registry-prometheus:1.6.4~~

### interlok-rest-metrics-profiler ###

#### Removed Dependencies ####
- ~~io.micrometer:micrometer-registry-prometheus:1.6.4~~

### interlok-rest-provider-datadog ###

#### Initial Dependencies ####
- io.micrometer:micrometer-registry-datadog:1.7.0

### interlok-rest-provider-prometheus ###

#### New Dependencies ####
- io.micrometer:micrometer-registry-prometheus:1.7.0

#### Updated Dependencies ####
- io.micrometer:micrometer-registry-prometheus:1.7.0 *(from 1.6.4)*

### interlok-service-tester-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.jayway.jsonpath:json-path:2.6.0

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*
- com.jayway.jsonpath:json-path:2.6.0 *(from 2.4.0)*

### interlok-service-tester-wiremock ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.github.tomakehurst:wiremock-jre8:2.28.0

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-core:2.12.3 *(from 2.12.2)*
- com.fasterxml.jackson.core:jackson-databind:2.12.3 *(from 2.12.2)*

#### Removed Dependencies ####
- ~~com.github.tomakehurst:wiremock:2.25.0~~

### interlok-sshtunnel ###

#### New Dependencies ####
- com.github.mwiede:jsch:0.1.63

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.1.63 *(from 0.1.62)*

### interlok-stubs ###

#### New Dependencies ####
- com.github.mwiede:jsch:0.1.63
- com.sun.mail:jakarta.mail:1.6.7
- com.thoughtworks.xstream:xstream:1.4.17
- commons-io:commons-io:2.10.0
- mysql:mysql-connector-java:8.0.25
- net.sf.saxon:Saxon-HE:10.5
- org.apache.activemq:activemq-broker:5.16.2
- org.apache.activemq:activemq-client:5.16.2
- org.apache.activemq:activemq-jaas:5.16.2
- org.apache.activemq:activemq-kahadb-store:5.16.2
- org.apache.commons:commons-pool2:2.10.0
- org.awaitility:awaitility:4.1.0
- org.bouncycastle:bcmail-jdk15on:1.69
- org.bouncycastle:bcpkix-jdk15on:1.69
- org.bouncycastle:bcprov-jdk15on:1.69
- org.eclipse.jetty.aggregate:jetty-all:9.4.42.v20210604
- org.jruby:jruby-complete:9.2.18.0
- org.mockito:mockito-core:3.11.1
- org.mockito:mockito-inline:3.11.1

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.1.63 *(from 0.1.62)*
- com.sun.mail:jakarta.mail:1.6.7 *(from 1.6.5)*
- com.thoughtworks.xstream:xstream:1.4.17 *(from 1.4.16)*
- commons-io:commons-io:2.10.0 *(from 2.8.0)*
- mysql:mysql-connector-java:8.0.25 *(from 8.0.23)*
- net.sf.saxon:Saxon-HE:10.5 *(from 10.3)*
- org.apache.activemq:activemq-broker:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-client:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-jaas:5.16.2 *(from 5.16.1)*
- org.apache.activemq:activemq-kahadb-store:5.16.2 *(from 5.16.1)*
- org.apache.commons:commons-pool2:2.10.0 *(from 2.9.0)*
- org.awaitility:awaitility:4.1.0 *(from 4.0.3)*
- org.bouncycastle:bcmail-jdk15on:1.69 *(from 1.68)*
- org.bouncycastle:bcpkix-jdk15on:1.69 *(from 1.68)*
- org.bouncycastle:bcprov-jdk15on:1.69 *(from 1.68)*
- org.eclipse.jetty.aggregate:jetty-all:9.4.42.v20210604 *(from 9.4.39.v20210325)*
- org.jruby:jruby-complete:9.2.18.0 *(from 9.2.16.0)*
- org.mockito:mockito-core:3.11.1 *(from 3.8.0)*
- org.mockito:mockito-inline:3.11.1 *(from 3.8.0)*

### interlok-swift ###

#### New Dependencies ####
- com.prowidesoftware:pw-swift-core:SRU2020-9.1.5

#### Updated Dependencies ####
- com.prowidesoftware:pw-swift-core:SRU2020-9.1.5 *(from SRU2020-9.1.3)*

### interlok-vcs-git ###

#### New Dependencies ####
- com.github.mwiede:jsch:0.1.63
- org.eclipse.jgit:org.eclipse.jgit.ssh.jsch:5.11.1.202105131744-r
- org.eclipse.jgit:org.eclipse.jgit:5.11.1.202105131744-r

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.1.63 *(from 0.1.62)*
- org.eclipse.jgit:org.eclipse.jgit.ssh.jsch:5.11.1.202105131744-r *(from 5.10.0.202012080955-r)*
- org.eclipse.jgit:org.eclipse.jgit:5.11.1.202105131744-r *(from 5.10.0.202012080955-r)*

### interlok-webservice-cxf ###

#### New Dependencies ####
- org.apache.cxf:cxf-rt-frontend-jaxws:3.4.3
- org.apache.cxf:cxf-rt-transports-http:3.4.3
- org.glassfish:javax.json:1.1.4

#### Updated Dependencies ####
- org.apache.cxf:cxf-rt-frontend-jaxws:3.4.3 *(from 3.4.2)*
- org.apache.cxf:cxf-rt-transports-http:3.4.3 *(from 3.4.2)*
- org.glassfish:javax.json:1.1.4 *(from 1.1.2)*

### interlok-xa-atomikos ###

#### New Dependencies ####
- org.awaitility:awaitility:4.1.0

#### Updated Dependencies ####
- org.awaitility:awaitility:4.1.0 *(from 4.0.3)*
