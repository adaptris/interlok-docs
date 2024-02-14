## Version 4.6.0-RELEASE ##

### interlok-activemq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.apache.activemq:activemq-amqp:5.17.2
- org.apache.activemq:activemq-broker:5.17.2
- org.apache.activemq:activemq-client:5.17.2
- org.apache.activemq:activemq-jaas:5.17.2
- org.apache.activemq:activemq-kahadb-store:5.17.2
- org.apache.activemq:activemq-mqtt:5.17.2
- org.apache.activemq:activemq-spring:5.17.2
- org.apache.activemq:activemq-stomp:5.17.2
- org.apache.qpid:proton-j:0.34.0
- org.springframework:spring-beans:5.3.23
- org.springframework:spring-context:5.3.23

### interlok-amqp ###

#### Updated Dependencies ####
- com.rabbitmq:amqp-client:5.16.0
- io.netty:netty-buffer:4.1.84.Final
- io.netty:netty-codec-http:4.1.84.Final
- io.netty:netty-codec:4.1.84.Final
- io.netty:netty-common:4.1.84.Final
- io.netty:netty-handler:4.1.84.Final
- io.netty:netty-transport-native-epoll:4.1.84.Final
- io.netty:netty-transport-native-kqueue:4.1.84.Final
- io.netty:netty-transport-native-unix-common:4.1.84.Final
- io.netty:netty-transport:4.1.84.Final
- org.apache.qpid:proton-j:0.34.0
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-apache-geode ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.apache.geode:geode-core:1.15.1
- org.apache.shiro:shiro-core:1.10.0
- org.slf4j:slf4j-api:2.0.3
- org.springframework:spring-web:5.3.23

### interlok-apache-http ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-apache-http-async ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-apache-http5 ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-artemis ###

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.84.Final
- io.netty:netty-codec-http:4.1.84.Final
- io.netty:netty-codec:4.1.84.Final
- io.netty:netty-common:4.1.84.Final
- io.netty:netty-handler:4.1.84.Final
- io.netty:netty-transport-native-epoll:4.1.84.Final
- io.netty:netty-transport-native-kqueue:4.1.84.Final
- io.netty:netty-transport-native-unix-common:4.1.84.Final
- io.netty:netty-transport:4.1.84.Final
- org.apache.activemq:artemis-jms-server:2.26.0
- org.apache.activemq:artemis-server:2.26.0
- org.apache.commons:commons-configuration2:2.8.0

### interlok-as400 ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-aws-common ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.319
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-sts:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

#### Removed Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-sts:1.12.228

### interlok-aws-kinesis ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.319
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-kinesis:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- io.netty:netty-bom:4.1.84.Final
- io.netty:netty-buffer:
- io.netty:netty-codec-http:
- io.netty:netty-codec:
- io.netty:netty-common:
- io.netty:netty-handler:
- io.netty:netty-transport-native-epoll:
- io.netty:netty-transport-native-kqueue:
- io.netty:netty-transport-native-unix-common:
- io.netty:netty-transport:
- org.apache.kafka:kafka-clients:2.8.2

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- com.google.protobuf:protobuf-java:3.21.7
- com.squareup.wire:wire-compiler:4.4.2
- com.squareup.wire:wire-schema:4.4.2
- org.apache.avro:avro:1.11.1
- org.jetbrains.kotlin:kotlin-bom:1.7.10
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

#### Removed Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-kinesis:1.12.228
- io.netty:netty-buffer:4.1.77.Final
- io.netty:netty-codec-http:4.1.77.Final
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-common:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final
- io.netty:netty-transport-native-kqueue:4.1.77.Final
- io.netty:netty-transport-native-unix-common:4.1.77.Final
- io.netty:netty-transport:4.1.77.Final

### interlok-aws-kinesis-sdk ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.319
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-kinesis:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

#### Removed Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-kinesis:1.12.228

### interlok-aws-kms ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.319
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-kms:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

#### Removed Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-kms:1.12.228

### interlok-aws-s3 ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.319
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-s3:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

#### Removed Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-s3:1.12.228

### interlok-aws-sns ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-bom:1.12.319
- com.amazonaws:aws-java-sdk-core:
- com.amazonaws:aws-java-sdk-sns:
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

#### Removed Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-sns:1.12.228

### interlok-aws-sqs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:

#### Updated Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.1.0
- com.amazonaws:aws-java-sdk-core:1.12.319
- com.amazonaws:aws-java-sdk-sqs:1.12.319
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-azure-core ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-xml:
- com.fasterxml.jackson.datatype:jackson-datatype-jsr310:
- io.netty:netty-resolver-dns:4.1.84.Final
- org.codehaus.woodstox:stax2-api:4.2.1

#### Updated Dependencies ####
- com.azure:azure-identity:1.5.5
- com.azure:azure-storage-file-datalake:12.13.0
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- com.google.code.gson:gson:2.9.1
- com.microsoft.azure:msal4j:1.13.2
- com.microsoft.graph:microsoft-graph:5.36.0
- com.squareup.okhttp3:okhttp:4.10.0
- com.squareup.okio:okio:3.2.0
- io.netty:netty-codec-http2:4.1.84.Final
- io.netty:netty-codec-http:4.1.84.Final
- io.netty:netty-codec:4.1.84.Final
- io.netty:netty-handler-proxy:4.1.84.Final
- io.netty:netty-handler:4.1.84.Final
- io.netty:netty-transport-native-epoll:4.1.84.Final
- io.netty:netty-transport-native-kqueue:4.1.84.Final
- io.netty:netty-transport-native-unix-common:4.1.84.Final
- org.slf4j:slf4j-api:2.0.3

### interlok-azure-cosmosdb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:slf4j-api:2.0.3

### interlok-azure-datalake ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-azure-mail ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-azure-onedrive ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-cassandra ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.datastax.cassandra:cassandra-driver-core:3.11.3
- com.datastax.cassandra:cassandra-driver-mapping:3.11.3
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- io.netty:netty-codec:4.1.84.Final
- io.netty:netty-handler:4.1.84.Final
- io.netty:netty-transport-native-epoll:4.1.84.Final
- org.slf4j:slf4j-api:2.0.3

### interlok-client ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-client-jmx ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-common ###

#### New Dependencies ####
- org.apache.logging.log4j:log4j-slf4j2-impl:2.19.0

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-1.2-api:2.19.0
- org.apache.logging.log4j:log4j-api:2.19.0
- org.apache.logging.log4j:log4j-core:2.19.0
- org.eclipse.jetty.aggregate:jetty-all:9.4.49.v20220914
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:jul-to-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

#### Removed Dependencies ####
- org.apache.logging.log4j:log4j-slf4j-impl:2.17.2

### interlok-core ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.2.4
- net.sf.saxon:Saxon-HE:11.4
- org.apache.activemq:activemq-client:5.17.2
- org.apache.commons:commons-text:1.10.0
- org.eclipse.jetty.aggregate:jetty-all:9.4.49.v20220914
- org.slf4j:slf4j-api:2.0.3

### interlok-csv ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-csv-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-csv-schema ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-edi-legacy ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-edi-stream ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-ehcache ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-elastic-common ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:
- org.apache.lucene:lucene-core:8.11.1
- org.elasticsearch:elasticsearch-x-content:7.17.6

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- joda-time:joda-time:2.12.0
- org.apache.logging.log4j:log4j-api:2.19.0
- org.elasticsearch:elasticsearch:7.17.6
- org.slf4j:slf4j-api:2.0.3
- org.yaml:snakeyaml:1.33

### interlok-elastic-rest ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:
- org.elasticsearch:elasticsearch-x-content:7.17.6

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- joda-time:joda-time:2.12.0
- org.apache.logging.log4j:log4j-api:2.19.0
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.17.6
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.6
- org.slf4j:slf4j-api:2.0.3
- org.yaml:snakeyaml:1.33

### interlok-elastic-sdk ###

#### Initial Dependencies ####
- co.elastic.clients:elasticsearch-java:7.17.6
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- com.jayway.jsonpath:json-path:2.7.0
- commons-collections:commons-collections:3.2.2
- joda-time:joda-time:2.12.0
- org.apache.logging.log4j:log4j-api:2.19.0
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.6
- org.elasticsearch:elasticsearch-x-content:7.17.6
- org.slf4j:slf4j-api:2.0.3
- org.yaml:snakeyaml:1.33

### interlok-excel ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-exec ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-expressions ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-failover ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-filesystem ###

#### Updated Dependencies ####
- org.apache.tika:tika-core:2.5.0
- org.json:json:20220924
- org.slf4j:slf4j-api:2.0.3

### interlok-flyway ###

#### Updated Dependencies ####
- org.flywaydb:flyway-core:8.5.13

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- com.google.cloud:google-cloud-pubsub:1.120.20
- com.google.code.gson:gson:2.9.1
- com.google.protobuf:protobuf-java-util:3.21.7
- com.google.protobuf:protobuf-java:3.21.7
- io.grpc:grpc-alts:1.50.0
- io.grpc:grpc-auth:1.50.0
- io.grpc:grpc-netty:1.50.0
- io.grpc:grpc-protobuf:1.50.0
- io.grpc:grpc-stub:1.50.0
- io.netty:netty-codec-http2:4.1.82.Final
- io.netty:netty-codec-http:4.1.82.Final
- io.netty:netty-codec:4.1.82.Final
- io.netty:netty-handler-proxy:4.1.82.Final
- io.netty:netty-handler:4.1.82.Final
- io.netty:netty-transport-native-epoll:4.1.82.Final

### interlok-hpcc ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-jclouds-aws-sts ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-jclouds-blobstore ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-jclouds-common ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-jdbc ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-jms-oracleaq ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-jms-sonicmq ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-jmx-activemq ###

#### Updated Dependencies ####
- org.apache.activemq:activemq-client:5.17.2
- org.slf4j:slf4j-api:2.0.3
- org.springframework:spring-aop:5.3.23
- org.springframework:spring-beans:5.3.23
- org.springframework:spring-context:5.3.23
- org.springframework:spring-core:5.3.23
- org.springframework:spring-jms:5.3.23

### interlok-jmx-amqp ###

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.84.Final
- io.netty:netty-codec-http:4.1.84.Final
- io.netty:netty-codec:4.1.84.Final
- io.netty:netty-common:4.1.84.Final
- io.netty:netty-handler:4.1.84.Final
- io.netty:netty-transport-native-epoll:4.1.84.Final
- io.netty:netty-transport-native-kqueue:4.1.84.Final
- io.netty:netty-transport-native-unix-common:4.1.84.Final
- io.netty:netty-transport:4.1.84.Final
- org.apache.qpid:proton-j:0.34.0
- org.slf4j:slf4j-api:2.0.3
- org.springframework:spring-aop:5.3.23
- org.springframework:spring-beans:5.3.23
- org.springframework:spring-context:5.3.23
- org.springframework:spring-core:5.3.23
- org.springframework:spring-jms:5.3.23

### interlok-jmx-jms-common ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3
- org.springframework:spring-aop:5.3.23
- org.springframework:spring-beans:5.3.23
- org.springframework:spring-context:5.3.23
- org.springframework:spring-core:5.3.23
- org.springframework:spring-jms:5.3.23

### interlok-jmx-jms-stubs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.apache.activemq:activemq-amqp:5.17.2
- org.apache.activemq:activemq-broker:5.17.2
- org.apache.activemq:activemq-jaas:5.17.2
- org.apache.activemq:activemq-kahadb-store:5.17.2
- org.slf4j:slf4j-api:2.0.3
- org.springframework:spring-aop:5.3.23
- org.springframework:spring-beans:5.3.23
- org.springframework:spring-context:5.3.23
- org.springframework:spring-core:5.3.23
- org.springframework:spring-jms:5.3.23

### interlok-jmx-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.16.0
- com.solacesystems:sol-jcsmp:10.16.0
- com.solacesystems:sol-jms:10.16.0
- org.slf4j:slf4j-api:2.0.3
- org.springframework:spring-aop:5.3.23
- org.springframework:spring-beans:5.3.23
- org.springframework:spring-context:5.3.23
- org.springframework:spring-core:5.3.23
- org.springframework:spring-jms:5.3.23

### interlok-jmx-sonicmq ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-jolokia ###

#### Updated Dependencies ####
- org.eclipse.jetty.aggregate:jetty-all:9.4.49.v20220914

### interlok-jq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- net.thisptr:jackson-jq-extra:1.0.0-preview.20220705
- net.thisptr:jackson-jq:1.0.0-preview.20220705
- org.slf4j:slf4j-api:2.0.3

### interlok-jruby ###

#### Updated Dependencies ####
- org.jruby:jruby:9.3.8.0
- org.slf4j:slf4j-api:2.0.3

### interlok-jslt ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- com.schibsted.spt.data:jslt:0.1.13
- org.slf4j:slf4j-api:2.0.3

### interlok-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.json:json:20220924
- org.slf4j:slf4j-api:2.0.3
- xom:xom:1.3.8

### interlok-json-streaming ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- com.google.code.gson:gson:2.9.1
- org.slf4j:slf4j-api:2.0.3

### interlok-json-web-token ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.json:json:20220924
- org.slf4j:slf4j-api:2.0.3

### interlok-jsr107-cache ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-kafka ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- io.netty:netty-codec:4.1.84.Final
- io.netty:netty-handler:4.1.84.Final
- io.netty:netty-transport-native-epoll:4.1.84.Final
- org.slf4j:slf4j-api:2.0.3

### interlok-kie ###

#### Updated Dependencies ####
- org.drools:drools-compiler:7.73.0.Final
- org.drools:drools-core:7.73.0.Final
- org.slf4j:slf4j-api:2.0.3

### interlok-licensing ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-licensing-demo ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-logging ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-api:2.19.0
- org.apache.logging.log4j:log4j-core:2.19.0

### interlok-mongodb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:slf4j-api:2.0.3

### interlok-mqtt ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-msmq-javonet ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-nats ###

#### Updated Dependencies ####
- io.nats:jnats:2.16.1

### interlok-oauth-azure ###

#### Updated Dependencies ####
- com.google.code.gson:gson:2.9.1
- com.nimbusds:nimbus-jose-jwt:9.25.4
- org.slf4j:slf4j-api:2.0.3

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.4
- com.google.auth:google-auth-library-oauth2-http:1.11.0
- org.slf4j:slf4j-api:2.0.3

### interlok-oauth-generic ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:slf4j-api:2.0.3

### interlok-oauth-salesforce ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.slf4j:slf4j-api:2.0.3

### interlok-okhttp ###

#### Updated Dependencies ####
- com.squareup.okhttp3:okhttp:4.10.0
- org.slf4j:slf4j-api:2.0.3

### interlok-pdf ###

#### New Dependencies ####
- org.apache.xmlgraphics:batik-extension:1.15
- org.apache.xmlgraphics:batik-transcoder:1.15

#### Updated Dependencies ####
- org.apache.pdfbox:fontbox:2.0.27
- org.apache.pdfbox:pdfbox-tools:2.0.27
- org.apache.pdfbox:pdfbox:2.0.27
- org.slf4j:slf4j-api:2.0.3

### interlok-pgp ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-profiler ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-rabbitmq ###

#### Updated Dependencies ####
- com.rabbitmq:amqp-client:5.16.0
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-rest-metrics-jvm ###

#### Updated Dependencies ####
- io.micrometer:micrometer-core:1.9.5

### interlok-rest-provider-datadog ###

#### Updated Dependencies ####
- io.micrometer:micrometer-registry-datadog:1.9.5

### interlok-rest-provider-prometheus ###

#### Updated Dependencies ####
- io.micrometer:micrometer-registry-prometheus:1.9.5

### interlok-sap ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-service-tester ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-service-tester-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-databind:

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- org.json:json:20220924
- org.skyscreamer:jsonassert:1.5.1
- org.slf4j:slf4j-api:2.0.3

### interlok-service-tester-wiremock ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- org.eclipse.jetty:jetty-bom:9.4.48.v20220622

#### Updated Dependencies ####
- com.fasterxml.jackson:jackson-bom:2.13.4.20221013
- com.github.tomakehurst:wiremock-jre8:2.34.0
- org.slf4j:slf4j-api:2.0.3

### interlok-service-tester-xml ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.16.0
- com.solacesystems:sol-jcsmp:10.16.0
- com.solacesystems:sol-jms:10.16.0
- org.slf4j:slf4j-api:2.0.3

### interlok-sshtunnel ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.2.4
- org.slf4j:slf4j-api:2.0.3

### interlok-stax ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-stubs ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-swift ###

#### Updated Dependencies ####
- com.prowidesoftware:pw-swift-core:SRU2021-9.2.18
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-tibco ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-triggered ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-vcs-git ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.2.4
- org.slf4j:slf4j-api:2.0.3

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- org.apache.cxf:cxf-rt-frontend-jaxws:3.5.4
- org.apache.cxf:cxf-rt-transports-http:3.5.4
- org.slf4j:slf4j-api:2.0.3

### interlok-webspheremq ###

#### Updated Dependencies ####
- com.ibm.mq:com.ibm.mq.allclient:9.3.0.1
- org.slf4j:jcl-over-slf4j:2.0.3
- org.slf4j:slf4j-api:2.0.3

### interlok-work-unit ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-xa-activemq ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-xa-atomikos ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-xa-jms ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-xa-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.16.0
- com.solacesystems:sol-jcsmp:10.16.0
- com.solacesystems:sol-jms:10.16.0
- org.slf4j:slf4j-api:2.0.3

### interlok-xa-tibco ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3

### interlok-xa-wmq ###

#### Updated Dependencies ####
- com.ibm.mq:com.ibm.mq.allclient:9.3.0.1
- org.slf4j:slf4j-api:2.0.3

### interlok-xml-security ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:2.0.3
