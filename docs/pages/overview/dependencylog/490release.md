## Version 4.9.0-RELEASE ##

### bip-services ###

#### Updated Dependencies ####
- net.minidev:json-smart:2.5.0
- org.slf4j:slf4j-api:2.0.7

### interlok-activemq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- com.google.guava:guava:32.1.1-jre
- org.apache.activemq:activemq-amqp:5.18.2
- org.apache.activemq:activemq-broker:5.18.2
- org.apache.activemq:activemq-client:5.18.2
- org.apache.activemq:activemq-jaas:5.18.2
- org.apache.activemq:activemq-kahadb-store:5.18.2
- org.apache.activemq:activemq-mqtt:5.18.2
- org.apache.activemq:activemq-spring:5.18.2
- org.apache.activemq:activemq-stomp:5.18.2

### interlok-amqp ###

#### New Dependencies ####
- javax.jms:javax.jms-api:2.0.1

#### Updated Dependencies ####
- com.rabbitmq:amqp-client:5.18.0
- io.netty:netty-buffer:4.1.96.Final
- io.netty:netty-codec-http:4.1.96.Final
- io.netty:netty-codec:4.1.96.Final
- io.netty:netty-common:4.1.96.Final
- io.netty:netty-handler:4.1.96.Final
- io.netty:netty-transport-native-epoll:4.1.96.Final
- io.netty:netty-transport-native-kqueue:4.1.96.Final
- io.netty:netty-transport-native-unix-common:4.1.96.Final
- io.netty:netty-transport:4.1.96.Final
- org.apache.qpid:qpid-java-build:6.1.7
- org.apache.qpid:qpid-jms-client:1.10.0
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-apache-geode ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- commons-codec:commons-codec:1.16.0
- org.apache.shiro:shiro-core:1.12.0
- org.jgroups:jgroups:5.2.16.Final
- org.slf4j:slf4j-api:2.0.7
- org.springframework:spring-web:5.3.27

### interlok-apache-http ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-apache-http-async ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-apache-http5 ###

#### New Dependencies ####
- commons-codec:commons-codec:1.16.0

#### Updated Dependencies ####
- org.apache.httpcomponents.client5:httpclient5:5.2.1
- org.slf4j:slf4j-api:2.0.7

### interlok-artemis ###

#### New Dependencies ####
- com.google.guava:guava:32.1.1-jre

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.96.Final
- io.netty:netty-codec-http:4.1.96.Final
- io.netty:netty-codec-socks:4.1.96.Final
- io.netty:netty-codec:4.1.96.Final
- io.netty:netty-common:4.1.96.Final
- io.netty:netty-handler-proxy:4.1.96.Final
- io.netty:netty-handler:4.1.96.Final
- io.netty:netty-transport-native-epoll:4.1.96.Final
- io.netty:netty-transport-native-kqueue:4.1.96.Final
- io.netty:netty-transport-native-unix-common:4.1.96.Final
- io.netty:netty-transport:4.1.96.Final
- org.apache.activemq:artemis-jms-server:2.30.0
- org.apache.activemq:artemis-server:2.30.0
- org.jgroups:jgroups:5.2.16.Final

### interlok-as400 ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-aws-common ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-sts:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.518
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

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
- com.amazonaws:amazon-kinesis-client:1.15.0
- com.amazonaws:amazon-kinesis-producer:0.15.7
- com.amazonaws:aws-java-sdk-bom:1.12.518
- com.charleskorn.kaml:kaml:0.55.0
- com.fasterxml.jackson:jackson-bom:2.15.2
- com.google.guava:guava:32.1.1-jre
- com.google.protobuf:protobuf-java:3.23.4
- com.squareup.wire:wire-compiler:4.8.0
- com.squareup.wire:wire-schema:4.8.0
- commons-codec:commons-codec:1.16.0
- io.netty:netty-bom:4.1.96.Final
- org.apache.avro:avro:1.11.2
- org.apache.kafka:kafka-clients:3.5.1
- org.jetbrains.kotlin:kotlin-bom:1.8.22
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-aws-kinesis-sdk ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-kinesis:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.518
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-aws-kms ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-kms:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.518
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-aws-s3 ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-s3:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.518
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-aws-sns ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-sns:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.518
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-aws-sqs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.518
- com.amazonaws:aws-java-sdk-sqs:1.12.518
- com.fasterxml.jackson:jackson-bom:2.15.2
- commons-codec:commons-codec:1.16.0
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-azure-core ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-xml:
- com.fasterxml.jackson.datatype:jackson-datatype-jsr310:

#### Updated Dependencies ####
- com.azure:azure-identity:1.9.2
- com.azure:azure-storage-file-datalake:12.16.0
- com.fasterxml.jackson:jackson-bom:2.15.2
- com.google.code.gson:gson:2.10.1
- com.google.guava:guava:32.1.1-jre
- com.microsoft.azure:msal4j:1.13.9
- com.microsoft.graph:microsoft-graph:5.66.0
- com.squareup.okhttp3:okhttp:4.11.0
- com.squareup.okio:okio:3.4.0
- commons-codec:commons-codec:1.16.0
- io.netty:netty-codec-http2:4.1.96.Final
- io.netty:netty-codec-http:4.1.96.Final
- io.netty:netty-codec:4.1.96.Final
- io.netty:netty-handler-proxy:4.1.96.Final
- io.netty:netty-handler:4.1.96.Final
- io.netty:netty-resolver-dns:4.1.96.Final
- io.netty:netty-transport-native-epoll:4.1.96.Final
- io.netty:netty-transport-native-kqueue:4.1.96.Final
- io.netty:netty-transport-native-unix-common:4.1.96.Final
- net.minidev:json-smart:2.5.0
- org.slf4j:slf4j-api:2.0.7

### interlok-azure-cosmosdb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- commons-codec:commons-codec:1.16.0
- org.slf4j:slf4j-api:2.0.7

### interlok-azure-datalake ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-azure-mail ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-azure-onedrive ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-cassandra ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- com.google.guava:guava:32.1.1-jre
- io.netty:netty-codec:4.1.96.Final
- io.netty:netty-handler:4.1.96.Final
- io.netty:netty-transport-native-epoll:4.1.96.Final
- org.slf4j:slf4j-api:2.0.7

### interlok-client ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-client-jmx ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-cluster-manager ###

#### Updated Dependencies ####
- org.jgroups:jgroups:5.2.16.Final

### interlok-common ###

#### Updated Dependencies ####
- commons-io:commons-io:2.13.0
- org.apache.commons:commons-lang3:3.13.0
- org.eclipse.jetty.aggregate:jetty-all:9.4.51.v20230217
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:jul-to-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-core ###

#### New Dependencies ####
- org.bouncycastle:bcmail-jdk18on:1.76
- org.bouncycastle:bcpkix-jdk18on:1.76
- org.bouncycastle:bcprov-jdk18on:1.76

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.2.10
- commons-io:commons-io:2.13.0
- org.apache.activemq:activemq-client:5.18.2
- org.apache.commons:commons-lang3:3.13.0
- org.eclipse.jetty.aggregate:jetty-all:9.4.51.v20230217
- org.slf4j:slf4j-api:2.0.7

#### Removed Dependencies ####
- org.bouncycastle:bcmail-jdk15on:1.70
- org.bouncycastle:bcpkix-jdk15on:1.70
- org.bouncycastle:bcprov-jdk15on:1.70

### interlok-csv ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-csv-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-csv-schema ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-edi-legacy ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-edi-stream ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-ehcache ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-elastic-common ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- joda-time:joda-time:2.12.5
- org.apache.commons:commons-csv:1.10.0
- org.apache.logging.log4j:log4j-api:2.20.0
- org.apache.lucene:lucene-core:9.7.0
- org.elasticsearch:elasticsearch-x-content:7.17.12
- org.elasticsearch:elasticsearch:7.17.12
- org.slf4j:slf4j-api:2.0.7
- org.yaml:snakeyaml:2.0

### interlok-elastic-rest ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- commons-codec:commons-codec:1.16.0
- joda-time:joda-time:2.12.5
- org.apache.httpcomponents:httpclient:4.5.14
- org.apache.logging.log4j:log4j-api:2.20.0
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.17.12
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.12
- org.elasticsearch:elasticsearch-x-content:7.17.12
- org.slf4j:slf4j-api:2.0.7
- org.yaml:snakeyaml:2.0

### interlok-elastic-sdk ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:

#### Updated Dependencies ####
- co.elastic.clients:elasticsearch-java:7.17.12
- com.fasterxml.jackson:jackson-bom:2.15.2
- joda-time:joda-time:2.12.5
- org.apache.logging.log4j:log4j-api:2.20.0
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.12
- org.elasticsearch:elasticsearch-x-content:7.17.12
- org.slf4j:slf4j-api:2.0.7
- org.yaml:snakeyaml:2.0

### interlok-excel ###

#### Updated Dependencies ####
- org.apache.commons:commons-compress:1.23.0
- org.slf4j:slf4j-api:2.0.7

### interlok-exec ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-expressions ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-failover ###

#### Updated Dependencies ####
- org.jgroups:jgroups:5.2.16.Final
- org.slf4j:slf4j-api:2.0.7

### interlok-filesystem ###

#### Updated Dependencies ####
- com.hierynomus:smbj:0.12.1
- org.apache.tika:tika-core:2.8.0
- org.json:json:20230618
- org.slf4j:slf4j-api:2.0.7

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- com.google.cloud:google-cloud-pubsub:1.124.0
- com.google.code.gson:gson:2.10.1
- com.google.guava:guava:32.1.1-jre
- com.google.protobuf:protobuf-java-util:3.23.4
- com.google.protobuf:protobuf-java:3.23.4
- commons-codec:commons-codec:1.16.0
- io.grpc:grpc-alts:1.57.0
- io.grpc:grpc-auth:1.57.0
- io.grpc:grpc-netty:1.57.0
- io.grpc:grpc-protobuf:1.57.0
- io.grpc:grpc-stub:1.57.0
- io.netty:netty-codec-http2:4.1.96.Final
- io.netty:netty-codec-http:4.1.96.Final
- io.netty:netty-codec:4.1.96.Final
- io.netty:netty-handler-proxy:4.1.96.Final
- io.netty:netty-handler:4.1.96.Final
- io.netty:netty-transport-native-epoll:4.1.96.Final

### interlok-hpcc ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-installer ###

#### Updated Dependencies ####
- org.gradle:gradle-tooling-api:7.6.1

### interlok-jclouds-aws-sts ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-jclouds-blobstore ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-jclouds-common ###

#### Updated Dependencies ####
- com.google.guava:guava:32.1.1-jre
- org.slf4j:slf4j-api:2.0.7

### interlok-jdbc ###

#### Updated Dependencies ####
- com.google.guava:guava:32.1.1-jre
- commons-codec:commons-codec:1.16.0
- org.slf4j:slf4j-api:2.0.7

### interlok-jms-oracleaq ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-jms-sonicmq ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-jmx-activemq ###

#### Updated Dependencies ####
- commons-io:commons-io:2.13.0
- org.apache.commons:commons-lang3:3.13.0
- org.slf4j:slf4j-api:2.0.7
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

### interlok-jmx-amqp ###

#### Updated Dependencies ####
- commons-io:commons-io:2.13.0
- io.netty:netty-buffer:4.1.96.Final
- io.netty:netty-codec-http:4.1.96.Final
- io.netty:netty-codec:4.1.96.Final
- io.netty:netty-common:4.1.96.Final
- io.netty:netty-handler:4.1.96.Final
- io.netty:netty-transport-native-epoll:4.1.96.Final
- io.netty:netty-transport-native-kqueue:4.1.96.Final
- io.netty:netty-transport-native-unix-common:4.1.96.Final
- io.netty:netty-transport:4.1.96.Final
- org.apache.commons:commons-lang3:3.13.0
- org.apache.qpid:qpid-jms-client:1.10.0
- org.slf4j:slf4j-api:2.0.7
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

### interlok-jmx-jms-common ###

#### Updated Dependencies ####
- commons-io:commons-io:2.13.0
- org.apache.commons:commons-lang3:3.13.0
- org.slf4j:slf4j-api:2.0.7
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

### interlok-jmx-jms-stubs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- commons-io:commons-io:2.13.0
- org.apache.commons:commons-lang3:3.13.0
- org.slf4j:slf4j-api:2.0.7
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

### interlok-jmx-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.21.0
- com.solacesystems:sol-jcsmp:10.21.0
- com.solacesystems:sol-jms:10.21.0
- commons-io:commons-io:2.13.0
- org.apache.commons:commons-lang3:3.13.0
- org.slf4j:slf4j-api:2.0.7
- org.springframework:spring-aop:5.3.27
- org.springframework:spring-beans:5.3.27
- org.springframework:spring-context:5.3.27
- org.springframework:spring-core:5.3.27
- org.springframework:spring-jms:5.3.27

### interlok-jmx-sonicmq ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-jolokia ###

#### Updated Dependencies ####
- org.eclipse.jetty.aggregate:jetty-all:9.4.51.v20230217

### interlok-jq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.slf4j:slf4j-api:2.0.7

### interlok-jruby ###

#### Updated Dependencies ####
- org.jruby:jruby:9.4.3.0
- org.slf4j:slf4j-api:2.0.7

### interlok-jslt ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.slf4j:slf4j-api:2.0.7

### interlok-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:

#### Updated Dependencies ####
- com.bazaarvoice.jolt:jolt-core:0.1.8
- com.bazaarvoice.jolt:json-utils:0.1.8
- com.fasterxml.jackson:jackson-bom:2.15.2
- com.google.guava:guava:32.1.1-jre
- net.minidev:json-smart:2.5.0
- org.json:json:20230618
- org.slf4j:slf4j-api:2.0.7
- xom:xom:1.3.9

### interlok-json-streaming ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- com.google.code.gson:gson:2.10.1
- org.slf4j:slf4j-api:2.0.7

### interlok-json-web-token ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- org.bouncycastle:bcpg-jdk18on:1.76
- org.bouncycastle:bcprov-jdk18on:1.76

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.json:json:20230618
- org.slf4j:slf4j-api:2.0.7

#### Removed Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.70
- org.bouncycastle:bcprov-jdk15on:1.70

### interlok-jsr107-cache ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-kafka ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- io.netty:netty-codec:4.1.96.Final
- io.netty:netty-handler:4.1.96.Final
- io.netty:netty-transport-native-epoll:4.1.96.Final
- org.apache.kafka:kafka-clients:3.5.1
- org.apache.kafka:kafka_2.13:3.5.1
- org.apache.zookeeper:zookeeper:3.8.2
- org.slf4j:slf4j-api:2.0.7

### interlok-kie ###

#### Updated Dependencies ####
- commons-codec:commons-codec:1.16.0
- org.slf4j:slf4j-api:2.0.7

### interlok-licensing ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-licensing-demo ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-mongodb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.mongodb:mongodb-driver:3.12.14
- org.slf4j:slf4j-api:2.0.7

### interlok-mqtt ###

#### Updated Dependencies ####
- commons-codec:commons-codec:1.16.0
- org.slf4j:slf4j-api:2.0.7

### interlok-msmq-javonet ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-nats ###

#### Updated Dependencies ####
- io.nats:jnats:2.16.13

### interlok-oauth-azure ###

#### Updated Dependencies ####
- com.google.code.gson:gson:2.10.1
- com.nimbusds:nimbus-jose-jwt:9.31
- net.minidev:json-smart:2.5.0
- org.slf4j:slf4j-api:2.0.7

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.15.2
- com.google.auth:google-auth-library-oauth2-http:1.19.0
- com.google.guava:guava:32.1.1-jre
- commons-codec:commons-codec:1.16.0
- org.slf4j:slf4j-api:2.0.7

### interlok-oauth-generic ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.slf4j:slf4j-api:2.0.7

### interlok-oauth-salesforce ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- commons-codec:commons-codec:1.16.0
- org.slf4j:slf4j-api:2.0.7

### interlok-okhttp ###

#### Updated Dependencies ####
- com.squareup.okhttp3:okhttp:4.11.0
- org.slf4j:slf4j-api:2.0.7

### interlok-pdf ###

#### Updated Dependencies ####
- com.google.guava:guava:32.1.1-jre
- commons-io:commons-io:2.13.0
- org.apache.pdfbox:fontbox:2.0.29
- org.apache.pdfbox:pdfbox-tools:2.0.29
- org.apache.pdfbox:pdfbox:2.0.29
- org.slf4j:slf4j-api:2.0.7

### interlok-pgp ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-profiler ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-proxy ###

#### Updated Dependencies ####
- org.apache.httpcomponents.client5:httpclient5:5.2.1

### interlok-rabbitmq ###

#### New Dependencies ####
- javax.jms:javax.jms-api:2.0.1

#### Updated Dependencies ####
- com.rabbitmq:amqp-client:5.18.0
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-rest-metrics-jvm ###

#### Updated Dependencies ####
- io.micrometer:micrometer-core:1.11.2

### interlok-rest-provider-datadog ###

#### Updated Dependencies ####
- io.micrometer:micrometer-registry-datadog:1.11.2

### interlok-rest-provider-prometheus ###

#### Updated Dependencies ####
- io.micrometer:micrometer-registry-prometheus:1.11.2

### interlok-sap ###

#### Updated Dependencies ####
- org.apache.ant:ant:1.10.13
- org.slf4j:slf4j-api:2.0.7

### interlok-service-tester ###

#### Updated Dependencies ####
- commons-io:commons-io:2.13.0
- org.slf4j:slf4j-api:2.0.7

### interlok-service-tester-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- org.json:json:20230618
- org.slf4j:slf4j-api:2.0.7

### interlok-service-tester-wiremock ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.15.2
- com.google.guava:guava:32.1.1-jre
- org.eclipse.jetty:jetty-bom:9.4.51.v20230217
- org.slf4j:slf4j-api:2.0.7

### interlok-service-tester-xml ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.21.0
- com.solacesystems:sol-jcsmp:10.21.0
- com.solacesystems:sol-jms:10.21.0
- org.slf4j:slf4j-api:2.0.7

### interlok-sshtunnel ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.2.10
- org.slf4j:slf4j-api:2.0.7

### interlok-stax ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-stubs ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-swift ###

#### Updated Dependencies ####
- com.prowidesoftware:pw-swift-core:SRU2022-9.3.15
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-tibco ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-triggered ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-vcs-git ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.2.10
- commons-codec:commons-codec:1.16.0
- org.slf4j:slf4j-api:2.0.7

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-webspheremq ###

#### Updated Dependencies ####
- com.ibm.mq:com.ibm.mq.allclient:9.3.3.0
- org.slf4j:jcl-over-slf4j:2.0.7
- org.slf4j:slf4j-api:2.0.7

### interlok-work-unit ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-xa-activemq ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-xa-atomikos ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-xa-jms ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-xa-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.21.0
- com.solacesystems:sol-jcsmp:10.21.0
- com.solacesystems:sol-jms:10.21.0
- org.slf4j:slf4j-api:2.0.7

### interlok-xa-tibco ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7

### interlok-xa-wmq ###

#### Updated Dependencies ####
- com.ibm.mq:com.ibm.mq.allclient:9.3.3.0
- org.slf4j:slf4j-api:2.0.7

### interlok-xml-security ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.7
