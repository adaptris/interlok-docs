## Version 5.0.0-RELEASE ##

### bip-services ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-json:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- net.minidev:json-smart:2.5.0
- org.json:json:20231013

### interlok-activemq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- com.google.guava:guava:32.1.3-jre

#### Unchanged Dependencies ####
- org.apache.activemq.protobuf:activemq-protobuf:1.1
- org.apache.activemq:activemq-amqp:5.18.3
- org.apache.activemq:activemq-broker:5.18.3
- org.apache.activemq:activemq-client:5.18.3
- org.apache.activemq:activemq-jaas:5.18.3
- org.apache.activemq:activemq-kahadb-store:5.18.3
- org.apache.activemq:activemq-mqtt:5.18.3
- org.apache.activemq:activemq-spring:5.18.3
- org.apache.activemq:activemq-stomp:5.18.3
- org.apache.qpid:proton-j:0.34.1
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27

### interlok-amqp ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- io.netty:netty-buffer:4.1.100.Final
- io.netty:netty-codec-http:4.1.100.Final
- io.netty:netty-codec:4.1.100.Final
- io.netty:netty-common:4.1.100.Final
- io.netty:netty-handler:4.1.100.Final
- io.netty:netty-transport-native-epoll:4.1.100.Final
- io.netty:netty-transport-native-kqueue:4.1.100.Final
- io.netty:netty-transport-native-unix-common:4.1.100.Final
- io.netty:netty-transport:4.1.100.Final
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:2.4.0
- com.rabbitmq:amqp-client:5.20.0
- org.apache.qpid:proton-j:0.34.1
- org.apache.qpid:qpid-client:6.4.0
- org.apache.qpid:qpid-java-build:6.1.7
- org.apache.qpid:qpid-jms-client:1.10.0

#### Removed Dependencies ####
- javax.jms:javax.jms-api:2.0.1

### interlok-apache-geode ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.apache.shiro:shiro-core:1.12.0
- org.jgroups:jgroups:5.3.0.Final
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- commons-beanutils:commons-beanutils:1.9.4
- commons-codec:commons-codec:1.16.0
- org.apache.geode:geode-core:1.15.1
- org.springframework:spring-web:5.3.27

### interlok-apache-http ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.14

### interlok-apache-http-async ###

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.apache.httpcomponents:httpasyncclient:4.1.5
- org.apache.httpcomponents:httpclient:4.5.14

### interlok-apache-http5 ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.apache.httpcomponents.client5:httpclient5:5.2.1
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.16.0

### interlok-artemis ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.google.guava:guava:32.1.3-jre
- io.netty:netty-buffer:4.1.100.Final
- io.netty:netty-codec-http:4.1.100.Final
- io.netty:netty-codec-socks:4.1.100.Final
- io.netty:netty-codec:4.1.100.Final
- io.netty:netty-common:4.1.100.Final
- io.netty:netty-handler-proxy:4.1.100.Final
- io.netty:netty-handler:4.1.100.Final
- io.netty:netty-transport-native-epoll:4.1.100.Final
- io.netty:netty-transport-native-kqueue:4.1.100.Final
- io.netty:netty-transport-native-unix-common:4.1.100.Final
- io.netty:netty-transport:4.1.100.Final
- org.jgroups:jgroups:5.3.0.Final

#### Unchanged Dependencies ####
- org.apache.activemq:artemis-jms-server:2.31.2
- org.apache.activemq:artemis-server:2.31.2
- org.apache.commons:commons-configuration2:2.9.0

### interlok-as400 ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- net.sf.jt400:jt400:9.1
- net.sf:cb2xml:0.92

### interlok-aws-common ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-sts:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.amazonaws:aws-java-sdk-bom:1.12.576
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

### interlok-aws-kinesis ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-kinesis:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- io.netty:netty-buffer:
- io.netty:netty-codec-http:
- io.netty:netty-codec:
- io.netty:netty-common:
- io.netty:netty-handler:
- io.netty:netty-transport-native-epoll:
- io.netty:netty-transport-native-kqueue:
- io.netty:netty-transport-native-unix-common:
- io.netty:netty-transport:

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.amazonaws:amazon-kinesis-producer:0.15.8
- com.amazonaws:aws-java-sdk-bom:1.12.576
- com.charleskorn.kaml:kaml:0.55.0
- com.fasterxml.jackson:jackson-bom:2.15.3
- com.google.guava:guava:32.1.3-jre
- com.google.protobuf:protobuf-java:3.25.0
- com.squareup.okio:okio-fakefilesystem:3.6.0
- com.squareup.okio:okio:3.6.0
- com.squareup.wire:wire-compiler:4.9.1
- com.squareup.wire:wire-schema:4.9.1
- io.netty:netty-bom:4.1.100.Final
- org.apache.commons:commons-compress:1.24.0
- org.apache.kafka:kafka-clients:3.6.0
- org.jetbrains.kotlin:kotlin-bom:1.8.22
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.amazonaws:amazon-kinesis-client:1.15.0
- commons-codec:commons-codec:1.16.0
- org.apache.avro:avro:1.11.3
- org.json:json:20231013

### interlok-aws-kinesis-sdk ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-kinesis:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.amazonaws:aws-java-sdk-bom:1.12.576
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

### interlok-aws-kms ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-kms:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.amazonaws:aws-java-sdk-bom:1.12.576
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

### interlok-aws-s3 ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-s3:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.amazonaws:aws-java-sdk-bom:1.12.576
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

### interlok-aws-sns ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-sns:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.amazonaws:aws-java-sdk-bom:1.12.576
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

### interlok-aws-sqs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.amazonaws:aws-java-sdk-core:1.12.576
- com.amazonaws:aws-java-sdk-sqs:1.12.576
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.1.0
- commons-codec:commons-codec:1.16.0
- org.apache.httpcomponents:httpclient:4.5.14

### interlok-aws2-common ###

#### Initial Dependencies ####
- com.adaptris:interlok-apache-http:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson.core:jackson-annotations:2.15.3
- com.fasterxml.jackson.core:jackson-core:2.15.3
- com.fasterxml.jackson.core:jackson-databind:2.15.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9
- software.amazon.awssdk:apache-client:2.21.15
- software.amazon.awssdk:sdk-core:2.21.15
- software.amazon.awssdk:sts:2.21.15

### interlok-aws2-kms ###

#### Initial Dependencies ####
- com.adaptris:interlok-aws2-common:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson.core:jackson-annotations:2.15.3
- com.fasterxml.jackson.core:jackson-core:2.15.3
- com.fasterxml.jackson.core:jackson-databind:2.15.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9
- software.amazon.awssdk:kms:2.21.15
- software.amazon.awssdk:sdk-core:2.21.15

### interlok-aws2-s3 ###

#### Initial Dependencies ####
- com.adaptris:interlok-aws2-common:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson.core:jackson-annotations:2.15.3
- com.fasterxml.jackson.core:jackson-core:2.15.3
- com.fasterxml.jackson.core:jackson-databind:2.15.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9
- software.amazon.awssdk:s3:2.21.15
- software.amazon.awssdk:sdk-core:2.21.15

### interlok-azure-core ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-xml:
- com.fasterxml.jackson.datatype:jackson-datatype-jsr310:

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.azure:azure-identity:1.10.4
- com.azure:azure-storage-file-datalake:12.17.1
- com.fasterxml.jackson:jackson-bom:2.15.3
- com.google.guava:guava:32.1.3-jre
- com.microsoft.azure:msal4j:1.14.0
- com.microsoft.graph:microsoft-graph:5.75.0
- com.squareup.okio:okio:3.6.0
- io.netty:netty-codec-http2:4.1.100.Final
- io.netty:netty-codec-http:4.1.100.Final
- io.netty:netty-codec:4.1.100.Final
- io.netty:netty-handler-proxy:4.1.100.Final
- io.netty:netty-handler:4.1.100.Final
- io.netty:netty-resolver-dns:4.1.100.Final
- io.netty:netty-transport-native-epoll:4.1.100.Final
- io.netty:netty-transport-native-kqueue:4.1.100.Final
- io.netty:netty-transport-native-unix-common:4.1.100.Final
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.google.code.gson:gson:2.10.1
- com.squareup.okhttp3:okhttp:4.12.0
- commons-codec:commons-codec:1.16.0
- net.minidev:json-smart:2.5.0
- org.codehaus.staxmate:stax2:2.1
- org.codehaus.woodstox:stax2-api:4.2.2

### interlok-azure-cosmosdb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.microsoft.azure:azure-documentdb:2.6.5
- commons-codec:commons-codec:1.16.0
- org.json:json:20231013

### interlok-azure-datalake ###

#### Updated Dependencies ####
- com.adaptris:interlok-azure-core:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-azure-mail ###

#### Updated Dependencies ####
- com.adaptris:interlok-azure-core:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-mail:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-azure-onedrive ###

#### Updated Dependencies ####
- com.adaptris:interlok-azure-core:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-boot ###

### interlok-cassandra ###

#### New Dependencies ####
- com.datastax.oss:java-driver-core:4.17.0
- com.datastax.oss:java-driver-mapper-runtime:4.17.0
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- com.google.guava:guava:32.1.3-jre
- io.netty:netty-codec:4.1.100.Final
- io.netty:netty-handler:4.1.100.Final
- io.netty:netty-transport-native-epoll:4.1.100.Final
- org.slf4j:slf4j-api:2.0.9

#### Removed Dependencies ####
- com.datastax.cassandra:cassandra-driver-core:3.11.5
- com.datastax.cassandra:cassandra-driver-mapping:3.11.5

### interlok-client ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-client-jmx ###

#### Updated Dependencies ####
- com.adaptris:interlok-client:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-cluster-manager ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.jgroups:jgroups:5.3.0.Final

### interlok-common ###

#### New Dependencies ####
- org.eclipse.jetty.http2:http2-client:10.0.18
- org.eclipse.jetty.http2:http2-common:10.0.18
- org.eclipse.jetty.http2:http2-hpack:10.0.18
- org.eclipse.jetty.http2:http2-server:10.0.18
- org.eclipse.jetty.websocket:websocket-javax-client:10.0.18
- org.eclipse.jetty.websocket:websocket-javax-server:10.0.18
- org.eclipse.jetty:jetty-alpn-client:10.0.18
- org.eclipse.jetty:jetty-alpn-java-client:10.0.18
- org.eclipse.jetty:jetty-alpn-java-server:10.0.18
- org.eclipse.jetty:jetty-alpn-server:10.0.18
- org.eclipse.jetty:jetty-annotations:10.0.18
- org.eclipse.jetty:jetty-client:10.0.18
- org.eclipse.jetty:jetty-deploy:10.0.18
- org.eclipse.jetty:jetty-http:10.0.18
- org.eclipse.jetty:jetty-io:10.0.18
- org.eclipse.jetty:jetty-jaspi:10.0.18
- org.eclipse.jetty:jetty-jmx:10.0.18
- org.eclipse.jetty:jetty-jndi:10.0.18
- org.eclipse.jetty:jetty-plus:10.0.18
- org.eclipse.jetty:jetty-quickstart:10.0.18
- org.eclipse.jetty:jetty-rewrite:10.0.18
- org.eclipse.jetty:jetty-security:10.0.18
- org.eclipse.jetty:jetty-server:10.0.18
- org.eclipse.jetty:jetty-servlet:10.0.18
- org.eclipse.jetty:jetty-servlets:10.0.18
- org.eclipse.jetty:jetty-util-ajax:10.0.18
- org.eclipse.jetty:jetty-util:10.0.18
- org.eclipse.jetty:jetty-webapp:10.0.18
- org.eclipse.jetty:jetty-xml:10.0.18

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- commons-io:commons-io:2.15.0
- org.apache.commons:commons-lang3:3.13.0
- org.apache.logging.log4j:log4j-1.2-api:2.21.1
- org.apache.logging.log4j:log4j-api:2.21.1
- org.apache.logging.log4j:log4j-core:2.21.1
- org.apache.logging.log4j:log4j-slf4j2-impl:2.21.1
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:jul-to-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.20
- commons-net:commons-net:3.10.0
- commons-pool:commons-pool:1.6
- javax.servlet:javax.servlet-api:4.0.1
- org.apache.commons:commons-pool2:2.12.0

#### Removed Dependencies ####
- org.eclipse.jetty.aggregate:jetty-all:9.4.53.v20231009

### interlok-core ###

#### New Dependencies ####
- org.eclipse.jetty.http2:http2-client:10.0.18
- org.eclipse.jetty.http2:http2-common:10.0.18
- org.eclipse.jetty.http2:http2-hpack:10.0.18
- org.eclipse.jetty.http2:http2-server:10.0.18
- org.eclipse.jetty.websocket:websocket-javax-client:10.0.18
- org.eclipse.jetty.websocket:websocket-javax-server:10.0.18
- org.eclipse.jetty:jetty-alpn-client:10.0.18
- org.eclipse.jetty:jetty-alpn-java-client:10.0.18
- org.eclipse.jetty:jetty-alpn-java-server:10.0.18
- org.eclipse.jetty:jetty-alpn-server:10.0.18
- org.eclipse.jetty:jetty-annotations:10.0.18
- org.eclipse.jetty:jetty-client:10.0.18
- org.eclipse.jetty:jetty-deploy:10.0.18
- org.eclipse.jetty:jetty-http:10.0.18
- org.eclipse.jetty:jetty-io:10.0.18
- org.eclipse.jetty:jetty-jaspi:10.0.18
- org.eclipse.jetty:jetty-jmx:10.0.18
- org.eclipse.jetty:jetty-jndi:10.0.18
- org.eclipse.jetty:jetty-plus:10.0.18
- org.eclipse.jetty:jetty-quickstart:10.0.18
- org.eclipse.jetty:jetty-rewrite:10.0.18
- org.eclipse.jetty:jetty-security:10.0.18
- org.eclipse.jetty:jetty-server:10.0.18
- org.eclipse.jetty:jetty-servlet:10.0.18
- org.eclipse.jetty:jetty-servlets:10.0.18
- org.eclipse.jetty:jetty-util-ajax:10.0.18
- org.eclipse.jetty:jetty-util:10.0.18
- org.eclipse.jetty:jetty-webapp:10.0.18
- org.eclipse.jetty:jetty-xml:10.0.18

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.github.mwiede:jsch:0.2.12
- commons-io:commons-io:2.15.0
- org.apache.commons:commons-exec:1.3
- org.apache.commons:commons-lang3:3.13.0
- org.bouncycastle:bcmail-jdk18on:1.76
- org.bouncycastle:bcpkix-jdk18on:1.76
- org.bouncycastle:bcprov-jdk18on:1.76
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.mchange:c3p0:0.9.5.5
- com.sun.activation:jakarta.activation:1.2.2
- com.sun.mail:jakarta.mail:1.6.7
- com.thoughtworks.xstream:xstream:1.4.20
- com.zaxxer:HikariCP:5.1.0
- commons-net:commons-net:3.10.0
- io.github.classgraph:classgraph:4.8.116
- jakarta.jms:jakarta.jms-api:2.0.3
- jakarta.validation:jakarta.validation-api:2.0.2
- javax.servlet:javax.servlet-api:4.0.1
- net.jodah:expiringmap:0.5.11
- net.sf.joost:joost:0.9.1
- net.sf.saxon:Saxon-HE:11.4
- org.apache-extras.beanshell:bsh:2.0b6
- org.apache.activemq:activemq-client:5.18.3
- org.apache.commons:commons-collections4:4.4
- org.apache.commons:commons-pool2:2.12.0
- org.apache.commons:commons-text:1.11.0
- org.apache.derby:derby:10.15.2.0
- org.apache.derby:derbytools:10.15.2.0
- org.codehaus.jettison:jettison:1.5.4
- org.flywaydb:flyway-core:8.5.13
- org.glassfish.external:opendmk_jdmkrt_jar:1.0-b01-ea
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.glassfish:jakarta.el:3.0.4
- org.hibernate.javax.persistence:hibernate-jpa-2.1-api:1.0.2.Final
- org.hibernate.validator:hibernate-validator:6.1.7.Final
- org.quartz-scheduler:quartz:2.3.2
- xerces:xercesImpl:2.12.2

#### Removed Dependencies ####
- org.eclipse.jetty.aggregate:jetty-all:9.4.53.v20231009

### interlok-core-apt ###

#### Unchanged Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.20
- jakarta.validation:jakarta.validation-api:2.0.2

### interlok-csv ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-stax:5.0.0-RELEASE
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- net.sf.supercsv:super-csv:2.4.0

### interlok-csv-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-csv:5.0.0-RELEASE
- com.adaptris:interlok-json:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

### interlok-csv-schema ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9
- uk.gov.nationalarchives:csv-validator-java-api:1.1.5

#### Unchanged Dependencies ####
- com.gilt:gfc-semver_2.11:0.0.5
- org.scala-lang.plugins:scala-continuations-library_2.11:1.0.3
- org.scala-lang:scala-library:2.11.12

### interlok-edi-legacy ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-edi-stream ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- javax.cache:cache-api:1.1.1

### interlok-ehcache ###

#### Updated Dependencies ####
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- net.sf.ehcache:ehcache:2.10.9.2

### interlok-elastic-common ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-csv:5.0.0-RELEASE
- com.adaptris:interlok-json:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- joda-time:joda-time:2.12.5
- org.apache.logging.log4j:log4j-api:2.21.1
- org.apache.lucene:lucene-core:9.8.0
- org.elasticsearch:elasticsearch-x-content:7.17.13
- org.elasticsearch:elasticsearch:7.17.13
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.8.0
- commons-collections:commons-collections:3.2.2
- net.sf.supercsv:super-csv:2.4.0
- org.apache.commons:commons-csv:1.10.0
- org.yaml:snakeyaml:2.2

#### Removed Dependencies ####
- org.apache.logging.log4j:log4j-core:2.22.1

### interlok-elastic-rest ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http-async:5.0.0-RELEASE
- com.adaptris:interlok-apache-http:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-elastic-common:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- joda-time:joda-time:2.12.5
- org.apache.logging.log4j:log4j-api:2.21.1
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.17.13
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.13
- org.elasticsearch:elasticsearch-x-content:7.17.13
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.8.0
- commons-codec:commons-codec:1.16.0
- commons-collections:commons-collections:3.2.2
- org.apache.httpcomponents:httpclient:4.5.14
- org.yaml:snakeyaml:2.2

#### Removed Dependencies ####
- org.apache.logging.log4j:log4j-core:2.22.1

### interlok-elastic-sdk ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:

#### Updated Dependencies ####
- co.elastic.clients:elasticsearch-java:7.17.13
- com.adaptris:interlok-apache-http-async:5.0.0-RELEASE
- com.adaptris:interlok-apache-http:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-elastic-common:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- joda-time:joda-time:2.12.5
- org.apache.logging.log4j:log4j-api:2.21.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.13
- org.elasticsearch:elasticsearch-x-content:7.17.13
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.8.0
- commons-collections:commons-collections:3.2.2
- org.yaml:snakeyaml:2.2

#### Removed Dependencies ####
- org.apache.logging.log4j:log4j-core:2.22.1
- org.eclipse.parsson:parsson:1.1.5

### interlok-excel ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.apache.commons:commons-compress:1.24.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.apache.poi:poi-ooxml:4.1.2
- org.apache.poi:poi:4.1.2

### interlok-exec ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.apache.commons:commons-exec:1.3
- org.slf4j:slf4j-api:2.0.9

### interlok-expressions ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.apache-extras.beanshell:bsh:2.0b6

### interlok-failover ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.jgroups:jgroups:5.3.0.Final
- org.slf4j:slf4j-api:2.0.9

### interlok-filesystem ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.hierynomus:smbj:0.12.2
- org.apache.commons:commons-compress:1.24.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.apache.tika:tika-core:2.9.1
- org.json:json:20231013

### interlok-flatfile ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE

### interlok-flyway ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE

#### Unchanged Dependencies ####
- commons-collections:commons-collections:3.2.2
- org.flywaydb:flyway-core:8.5.13

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-oauth-gcloud:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- com.google.cloud:google-cloud-pubsub:1.125.9
- com.google.protobuf:protobuf-java-util:3.24.4
- com.google.protobuf:protobuf-java:3.24.4
- io.grpc:grpc-alts:1.59.0
- io.grpc:grpc-auth:1.59.0
- io.grpc:grpc-context:1.59.0
- io.grpc:grpc-googleapis:1.59.0
- io.grpc:grpc-inprocess:1.59.0
- io.grpc:grpc-netty:1.59.0
- io.grpc:grpc-protobuf:1.59.0
- io.grpc:grpc-services:1.59.0
- io.grpc:grpc-stub:1.59.0
- io.netty:netty-codec-http2:4.1.100.Final
- io.netty:netty-codec-http:4.1.100.Final
- io.netty:netty-codec:4.1.100.Final
- io.netty:netty-handler-proxy:4.1.100.Final
- io.netty:netty-handler:4.1.100.Final
- io.netty:netty-transport-native-epoll:4.1.100.Final

#### Unchanged Dependencies ####
- com.google.code.gson:gson:2.10.1
- com.google.guava:guava:32.1.1-jre
- commons-codec:commons-codec:1.16.0
- org.apache.httpcomponents:httpclient:4.5.14

### interlok-hpcc ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.apache.commons:commons-exec:1.3
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- oro:oro:2.0.8

### interlok-installer ###

#### Unchanged Dependencies ####
- org.gradle:gradle-tooling-api:7.6.1
- org.openjfx:javafx-base:11.0.2
- org.openjfx:javafx-controls:11.0.2
- org.openjfx:javafx-fxml:11.0.2
- org.openjfx:javafx-graphics:11.0.2

### interlok-jclouds-aws-sts ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-jclouds-common:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.apache.jclouds.api:sts:2.5.0

### interlok-jclouds-blobstore ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-jclouds-common:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- javax.xml.bind:jaxb-api:2.3.1
- org.apache.jclouds:jclouds-blobstore:2.5.0

### interlok-jclouds-common ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.google.guava:guava:32.1.3-jre
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.apache.jclouds:jclouds-core:2.5.0

### interlok-jdbc ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.google.guava:guava:32.1.3-jre
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.16.0
- org.codehaus.staxmate:stax2:2.1

### interlok-jms-oracleaq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.oracle:ojdbc14:10.2.0.1.0
- com.oracle:oracle-aq:1.0

### interlok-jms-sonicmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.aurea:sonic-channel:8.5.0
- com.aurea:sonic-client:8.5.0
- com.aurea:sonic-crypto:8.5.0
- com.aurea:sonic-xa:8.5.0
- com.aurea:sonic-xmessage:8.5.0

### interlok-jms3-common ###

#### Initial Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- io.netty:netty-bom:4.1.100.Final
- jakarta.jms:jakarta.jms-api:3.1.0
- org.apache.activemq:artemis-jakarta-client:2.31.2
- org.apache.geronimo.specs:geronimo-jms_2.0_spec:1.0-alpha-2
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

### interlok-jmx-activemq ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:5.0.0-RELEASE
- commons-io:commons-io:2.15.0
- org.apache.activemq:activemq-client:5.17.4
- org.apache.commons:commons-lang3:3.13.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.20
- commons-lang:commons-lang:2.6
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

### interlok-jmx-amqp ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:5.0.0-RELEASE
- commons-io:commons-io:2.15.0
- io.netty:netty-buffer:4.1.100.Final
- io.netty:netty-codec-http:4.1.100.Final
- io.netty:netty-codec:4.1.100.Final
- io.netty:netty-common:4.1.100.Final
- io.netty:netty-handler:4.1.100.Final
- io.netty:netty-transport-native-epoll:4.1.100.Final
- io.netty:netty-transport-native-kqueue:4.1.100.Final
- io.netty:netty-transport-native-unix-common:4.1.100.Final
- io.netty:netty-transport:4.1.100.Final
- org.apache.commons:commons-lang3:3.13.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.20
- commons-lang:commons-lang:2.6
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.qpid:proton-j:0.34.1
- org.apache.qpid:proton-jms:0.12.2
- org.apache.qpid:qpid-jms-client:1.10.0
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

### interlok-jmx-jms-common ###

#### Updated Dependencies ####
- commons-io:commons-io:2.15.0
- org.apache.commons:commons-lang3:3.13.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.20
- commons-lang:commons-lang:2.6
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

### interlok-jmx-jms-stubs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- org.junit.jupiter:junit-jupiter-engine:5.10.0

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- commons-io:commons-io:2.15.0
- org.apache.activemq:activemq-amqp:5.17.4
- org.apache.activemq:activemq-broker:5.17.4
- org.apache.activemq:activemq-jaas:5.17.4
- org.apache.activemq:activemq-kahadb-store:5.17.4
- org.apache.commons:commons-lang3:3.13.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.20
- commons-lang:commons-lang:2.6
- javax.management.j2ee:javax.management.j2ee-api:1.1.2
- org.apache.activemq.protobuf:activemq-protobuf:1.1
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

#### Removed Dependencies ####
- junit:junit:4.13.2

### interlok-jmx-solace ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:5.0.0-RELEASE
- com.solacesystems:sol-common:10.21.0
- com.solacesystems:sol-jcsmp:10.21.0
- com.solacesystems:sol-jms:10.21.0
- commons-io:commons-io:2.15.0
- org.apache.commons:commons-lang3:3.13.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.20
- commons-lang:commons-lang:2.6
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

### interlok-jmx-sonicmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:5.0.0-RELEASE
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.aurea:sonic-channel:8.5.0
- com.aurea:sonic-client:8.5.0
- com.aurea:sonic-crypto:8.5.0
- com.aurea:sonic-xa:8.5.0
- com.aurea:sonic-xmessage:8.5.0

### interlok-jolokia ###

#### New Dependencies ####
- org.eclipse.jetty:jetty-bom:10.0.18

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE

#### Unchanged Dependencies ####
- org.jolokia:jolokia-core:1.7.2
- org.jolokia:jolokia-jsr160:1.7.2

#### Removed Dependencies ####
- org.eclipse.jetty.aggregate:jetty-all:9.4.53.v20231009

### interlok-jq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- net.thisptr:jackson-jq-extra:1.0.0-preview.20230409
- net.thisptr:jackson-jq:1.0.0-preview.20230409

### interlok-jruby ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.jruby:jruby:9.4.4.0
- org.slf4j:slf4j-api:2.0.9

### interlok-jslt ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.schibsted.spt.data:jslt:0.1.14

### interlok-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- com.flipkart.zjsonpatch:zjsonpatch:0.4.14
- com.github.erosb:everit-json-schema:1.14.3
- com.google.guava:guava:32.1.3-jre
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.bazaarvoice.jolt:jolt-core:0.1.8
- com.bazaarvoice.jolt:json-utils:0.1.8
- com.jayway.jsonpath:json-path:2.8.0
- commons-beanutils:commons-beanutils:1.9.4
- commons-collections:commons-collections:3.2.2
- net.minidev:json-smart:2.5.0
- net.sf.json-lib:json-lib:2.4
- org.json:json:20231013
- xerces:xercesImpl:2.12.2
- xom:xom:1.3.9

### interlok-json-streaming ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-json:5.0.0-RELEASE
- com.adaptris:interlok-stax:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- com.github.jsurfer:jsurfer-core:1.6.4
- com.github.jsurfer:jsurfer-gson:1.6.4
- com.github.jsurfer:jsurfer-jackson:1.6.4
- com.github.jsurfer:jsurfer-jsonsimple:1.6.4
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.google.code.gson:gson:2.10.1
- de.odysseus.staxon:staxon:1.3

### interlok-json-web-token ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.bouncycastle:bcpg-jdk18on:1.76
- org.bouncycastle:bcprov-jdk18on:1.76
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- io.jsonwebtoken:jjwt-api:0.12.3
- io.jsonwebtoken:jjwt-impl:0.12.3
- io.jsonwebtoken:jjwt-jackson:0.12.3
- org.json:json:20231013

### interlok-jsr107-cache ###

#### Updated Dependencies ####
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- javax.cache:cache-api:1.1.1

### interlok-kafka ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- io.netty:netty-codec:4.1.100.Final
- io.netty:netty-handler:4.1.100.Final
- io.netty:netty-transport-native-epoll:4.1.100.Final
- org.apache.kafka:kafka-clients:3.6.0
- org.apache.kafka:kafka_2.13:3.6.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- commons-collections:commons-collections:3.2.2
- org.apache.zookeeper:zookeeper:3.9.1

#### Removed Dependencies ####
- ch.qos.logback:logback-classic:1.2.13

### interlok-kie ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.20
- commons-codec:commons-codec:1.16.0
- org.apache.commons:commons-collections4:4.4
- org.drools:drools-compiler:7.73.0.Final
- org.drools:drools-core:7.73.0.Final

### interlok-licensing ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-licensing-demo ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-logging ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-api:2.21.1
- org.apache.logging.log4j:log4j-core:2.21.1

### interlok-mail ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE

#### Unchanged Dependencies ####
- com.sun.mail:jakarta.mail:1.6.7

### interlok-mongodb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-json:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.mongodb:mongodb-driver:3.12.14

### interlok-mqtt ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.16.0
- javax.transaction:jta:1.1
- org.apache.httpcomponents:httpclient:4.5.14
- org.eclipse.paho:org.eclipse.paho.client.mqttv3:1.2.5

### interlok-msmq-javonet ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.javonet:javonet:1.4-hf15

### interlok-nats ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- io.nats:jnats:2.17.1

### interlok-oauth-azure ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.nimbusds:nimbus-jose-jwt:9.37
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.google.code.gson:gson:2.10.1
- com.microsoft.azure:adal4j:1.6.7
- net.minidev:json-smart:2.5.0

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson.core:jackson-core:2.15.3
- com.google.auth:google-auth-library-oauth2-http:1.20.0
- com.google.guava:guava:32.1.3-jre
- io.grpc:grpc-context:1.59.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.16.0
- org.apache.httpcomponents:httpclient:4.5.14

### interlok-oauth-generic ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:5.0.0-RELEASE
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.8.0

### interlok-oauth-salesforce ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.16.0
- org.apache.httpcomponents:httpclient:4.5.14

### interlok-okhttp ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.squareup.okio:okio:3.6.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.squareup.okhttp3:okhttp:4.12.0

### interlok-pdf ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.google.guava:guava:32.1.3-jre
- commons-io:commons-io:2.15.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- net.sf.cssbox:pdf2dom:2.0.3
- org.apache.pdfbox:fontbox:2.0.29
- org.apache.pdfbox:pdfbox-tools:2.0.29
- org.apache.pdfbox:pdfbox:2.0.29
- org.apache.xmlgraphics:batik-extension:1.17
- org.apache.xmlgraphics:batik-transcoder:1.17
- org.apache.xmlgraphics:fop:2.9
- xerces:xercesImpl:2.12.2

### interlok-pgp ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.70
- org.bouncycastle:bcprov-jdk15on:1.70

### interlok-profiler ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.aspectj:aspectjrt:1.9.20.1
- org.aspectj:aspectjtools:1.9.20.1
- org.aspectj:aspectjweaver:1.9.20.1
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.apache.commons:commons-math3:3.6.1

### interlok-proxy ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:5.0.0-RELEASE
- com.adaptris:interlok-client:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.apache.httpcomponents.client5:httpclient5:5.2.1

### interlok-rabbitmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.rabbitmq:amqp-client:5.20.0

#### Removed Dependencies ####
- javax.jms:javax.jms-api:2.0.1

### interlok-rest-base ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:5.0.0-RELEASE
- com.adaptris:interlok-client:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE

### interlok-rest-cluster ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:5.0.0-RELEASE
- com.adaptris:interlok-client:5.0.0-RELEASE
- com.adaptris:interlok-cluster-manager:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-rest-base:5.0.0-RELEASE

### interlok-rest-health-check ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:5.0.0-RELEASE
- com.adaptris:interlok-client:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-rest-base:5.0.0-RELEASE

### interlok-rest-metrics-jvm ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:5.0.0-RELEASE
- com.adaptris:interlok-client:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-rest-base:5.0.0-RELEASE
- io.micrometer:micrometer-core:1.11.5

#### Unchanged Dependencies ####
- io.github.mweirauch:micrometer-jvm-extras:0.2.2

### interlok-rest-metrics-profiler ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:5.0.0-RELEASE
- com.adaptris:interlok-client:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-profiler:5.0.0-RELEASE
- com.adaptris:interlok-rest-base:5.0.0-RELEASE
- com.adaptris:interlok-rest-metrics-jvm:5.0.0-RELEASE

### interlok-rest-provider-datadog ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:5.0.0-RELEASE
- com.adaptris:interlok-client:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-rest-base:5.0.0-RELEASE
- com.adaptris:interlok-rest-metrics-jvm:5.0.0-RELEASE
- io.micrometer:micrometer-registry-datadog:1.11.5

### interlok-rest-provider-prometheus ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:5.0.0-RELEASE
- com.adaptris:interlok-client:5.0.0-RELEASE
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-rest-base:5.0.0-RELEASE
- com.adaptris:interlok-rest-metrics-jvm:5.0.0-RELEASE
- io.micrometer:micrometer-registry-prometheus:1.11.5

### interlok-sap ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.sap:sapidoc3:3.0.12
- com.sap:sapjco3:3.0.13
- org.apache.ant:ant:1.10.14

### interlok-scripting ###

#### Initial Dependencies ####
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.graalvm.js:js-scriptengine:23.0.2
- org.graalvm.js:js:23.0.2
- org.graalvm.sdk:graal-sdk:23.0.2
- org.slf4j:slf4j-api:2.0.9

### interlok-service-tester ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-varsub:5.0.0-RELEASE
- com.adaptris:interlok-xinclude:5.0.0-RELEASE
- commons-io:commons-io:2.15.0
- org.slf4j:slf4j-api:2.0.9

### interlok-service-tester-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-service-tester:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.8.0
- org.json:json:20231013
- org.skyscreamer:jsonassert:1.5.1

### interlok-service-tester-wiremock ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- io.netty:netty-bom:4.1.100.Final
- io.swagger.parser.v3:swagger-parser:2.1.18
- org.mock-server:mockserver-netty:5.15.0
- org.mozilla:rhino:1.7.14
- org.yaml:snakeyaml:2.2

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-service-tester:5.0.0-RELEASE
- com.fasterxml.jackson:jackson-bom:2.15.3
- com.google.guava:guava:32.1.3-jre
- org.eclipse.jetty:jetty-bom:10.0.18
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.8.0
- commons-fileupload:commons-fileupload:1.5

#### Removed Dependencies ####
- com.github.tomakehurst:wiremock-jre8:2.35.1
- org.json:json:20231013

### interlok-service-tester-xml ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-service-tester:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- xmlunit:xmlunit:1.6

### interlok-solace ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.solacesystems:sol-common:10.21.0
- com.solacesystems:sol-jcsmp:10.21.0
- com.solacesystems:sol-jms:10.21.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- net.jodah:expiringmap:0.5.11

### interlok-sshtunnel ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.github.mwiede:jsch:0.2.12
- org.slf4j:slf4j-api:2.0.9

### interlok-stax ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-stubs ###

#### New Dependencies ####
- org.junit.jupiter:junit-jupiter-api:5.10.1
- org.junit.jupiter:junit-jupiter-engine:5.10.1

#### Updated Dependencies ####
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Removed Dependencies ####
- junit:junit:4.13.2

### interlok-swift ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.prowidesoftware:pw-swift-core:SRU2022-9.3.15

### interlok-tibco ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.tibco:tibjms:6.3.0
- com.tibco:tibrv:7.5.1

### interlok-triggered ###

#### New Dependencies ####
- com.adaptris:interlok-licensing:5.0.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-varsub ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE

### interlok-vcs-git ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.github.mwiede:jsch:0.2.12
- org.eclipse.jgit:org.eclipse.jgit.ssh.jsch:6.7.0.202309050840-r
- org.eclipse.jgit:org.eclipse.jgit:6.7.0.202309050840-r
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.16.0
- commons-lang:commons-lang:2.6
- org.apache.httpcomponents:httpclient:4.5.14

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.sun.xml.messaging.saaj:saaj-impl:1.5.1
- jakarta.xml.bind:jakarta.xml.bind-api:2.3.2
- javax.jws:jsr181-api:1.0-MR1
- javax.xml.soap:saaj-api:1.3.5
- javax.xml.ws:jaxws-api:2.3.1
- org.apache.cxf:cxf-rt-frontend-jaxws:3.5.5
- org.apache.cxf:cxf-rt-transports-http:3.5.5
- org.eclipse:yasson:1.0.1
- org.glassfish.jaxb:jaxb-runtime:2.3.8
- org.glassfish:javax.json:1.1.4

### interlok-webspheremq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.ibm.mq:com.ibm.mq.allclient:9.3.4.0
- org.slf4j:jcl-over-slf4j:2.0.9
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.apache.geronimo.specs:geronimo-j2ee-connector_1.6_spec:1.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.json:json:20231013

### interlok-work-unit ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-varsub:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-xa-activemq ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- com.adaptris:interlok-xa-jms:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-xa-atomikos ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- com.adaptris:interlok-xa-jms:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.atomikos:transactions-jms:3.8.0
- org.awaitility:awaitility:4.2.0

### interlok-xa-jms ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

### interlok-xa-solace ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- com.adaptris:interlok-solace:5.0.0-RELEASE
- com.adaptris:interlok-xa-jms:5.0.0-RELEASE
- com.solacesystems:sol-common:10.21.0
- com.solacesystems:sol-jcsmp:10.21.0
- com.solacesystems:sol-jms:10.21.0
- org.slf4j:slf4j-api:2.0.9

### interlok-xa-tibco ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- com.adaptris:interlok-tibco:5.0.0-RELEASE
- com.adaptris:interlok-xa-jms:5.0.0-RELEASE
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- com.tibco:tibjms:6.3.0
- com.tibco:tibrv:7.5.1

### interlok-xa-wmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
- com.adaptris:interlok-licensing:5.0.0-RELEASE
- com.adaptris:interlok-webspheremq:5.0.0-RELEASE
- com.adaptris:interlok-xa-jms:5.0.0-RELEASE
- com.ibm.mq:com.ibm.mq.allclient:9.3.4.0
- org.slf4j:slf4j-api:2.0.9

#### Unchanged Dependencies ####
- org.json:json:20231013

### interlok-xinclude ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:5.0.0-RELEASE
- com.adaptris:interlok-core:5.0.0-RELEASE
