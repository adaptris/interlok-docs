## Version 4.5.0-RELEASE ##

### interlok-activemq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.google.guava:guava:31.1-jre
- org.apache.activemq:activemq-amqp:5.17.1
- org.apache.activemq:activemq-broker:5.17.1
- org.apache.activemq:activemq-client:5.17.1
- org.apache.activemq:activemq-jaas:5.17.1
- org.apache.activemq:activemq-kahadb-store:5.17.1
- org.apache.activemq:activemq-mqtt:5.17.1
- org.apache.activemq:activemq-spring:5.17.1
- org.apache.activemq:activemq-stomp:5.17.1
- org.springframework:spring-beans:5.3.20
- org.springframework:spring-context:5.3.20

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-amqp ###

#### Updated Dependencies ####
- com.rabbitmq:amqp-client:5.14.2
- io.netty:netty-buffer:4.1.77.Final
- io.netty:netty-codec-http:4.1.77.Final
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-common:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final
- io.netty:netty-transport-native-kqueue:4.1.77.Final
- io.netty:netty-transport-native-unix-common:4.1.77.Final
- io.netty:netty-transport:4.1.77.Final
- org.apache.qpid:qpid-jms-client:1.6.0
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-apache-geode ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3
- org.jgroups:jgroups:4.2.4.Final
- org.springframework:spring-web:5.3.20

#### Updated Dependencies ####
- org.apache.geode:geode-core:1.14.4
- org.apache.shiro:shiro-core:1.9.0
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-apache-http ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-apache-http-async ###

#### Initial Dependencies ####
- org.apache.httpcomponents:httpasyncclient:4.1.5
- org.apache.httpcomponents:httpclient:4.5.13
- org.slf4j:slf4j-api:1.7.36

### interlok-apache-http5 ###

#### Updated Dependencies ####
- org.apache.httpcomponents.client5:httpclient5:5.1.3
- org.slf4j:slf4j-api:1.7.36

### interlok-artemis ###

#### New Dependencies ####
- org.jgroups:jgroups:4.2.4.Final

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.77.Final
- io.netty:netty-codec-http:4.1.77.Final
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-common:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final
- io.netty:netty-transport-native-kqueue:4.1.77.Final
- io.netty:netty-transport-native-unix-common:4.1.77.Final
- io.netty:netty-transport:4.1.77.Final
- org.apache.activemq:artemis-jms-server:2.22.0
- org.apache.activemq:artemis-server:2.22.0

### interlok-as400 ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-aws-common ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-sts:1.12.228
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1

### interlok-aws-kinesis ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson:jackson-bom:2.13.3
- com.squareup.wire:wire-compiler:4.3.0
- com.squareup.wire:wire-schema:4.3.0
- org.jetbrains.kotlin:kotlin-bom:1.4.32

#### Updated Dependencies ####
- com.amazonaws:amazon-kinesis-client:1.14.8
- com.amazonaws:amazon-kinesis-producer:0.14.12
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-kinesis:1.12.228
- com.google.guava:guava:31.1-jre
- com.google.protobuf:protobuf-java:3.20.1
- io.netty:netty-buffer:4.1.77.Final
- io.netty:netty-codec-http:4.1.77.Final
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-common:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final
- io.netty:netty-transport-native-kqueue:4.1.77.Final
- io.netty:netty-transport-native-unix-common:4.1.77.Final
- io.netty:netty-transport:4.1.77.Final
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1

### interlok-aws-kinesis-sdk ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-kinesis:1.12.228
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1

### interlok-aws-kms ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-kms:1.12.228
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1

### interlok-aws-s3 ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-s3:1.12.228
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1

### interlok-aws-sns ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-sns:1.12.228
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1

### interlok-aws-sqs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-sqs:1.12.228
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1

### interlok-azure-core ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-xml:
- com.fasterxml.jackson.datatype:jackson-datatype-jsr310:
- com.fasterxml.jackson:jackson-bom:2.13.3
- com.google.code.gson:gson:2.9.0
- com.squareup.okhttp3:okhttp:4.9.3
- com.squareup.okio:okio:3.1.0

#### Updated Dependencies ####
- com.azure:azure-identity:1.5.1
- com.azure:azure-storage-file-datalake:12.10.0
- com.google.guava:guava:31.1-jre
- com.microsoft.azure:msal4j:1.12.0
- io.netty:netty-codec-http2:4.1.77.Final
- io.netty:netty-codec-http:4.1.77.Final
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-handler-proxy:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final
- io.netty:netty-transport-native-kqueue:4.1.77.Final
- io.netty:netty-transport-native-unix-common:4.1.77.Final
- net.minidev:json-smart:2.4.8
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-xml:2.13.1
- com.fasterxml.jackson.datatype:jackson-datatype-jsr310:2.13.1

### interlok-azure-cosmosdb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-azure-datalake ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-azure-mail ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-azure-onedrive ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-cassandra ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.datastax.cassandra:cassandra-driver-core:3.11.1
- com.datastax.cassandra:cassandra-driver-mapping:3.11.1
- com.google.guava:guava:31.1-jre
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-client ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-client-jmx ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-common ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-1.2-api:2.17.2
- org.apache.logging.log4j:log4j-api:2.17.2
- org.apache.logging.log4j:log4j-core:2.17.2
- org.apache.logging.log4j:log4j-slf4j-impl:2.17.2
- org.eclipse.jetty.aggregate:jetty-all:9.4.46.v20220331
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:jul-to-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-core ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.2.1
- net.sf.saxon:Saxon-HE:11.3
- org.apache.activemq:activemq-client:5.17.1
- org.eclipse.jetty.aggregate:jetty-all:9.4.46.v20220331
- org.slf4j:slf4j-api:1.7.36

### interlok-csv ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-csv-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-csv-schema ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-edi-legacy ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-edi-stream ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-ehcache ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-elastic-common ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:
- com.fasterxml.jackson:jackson-bom:2.13.3
- org.elasticsearch:elasticsearch:7.15.1

#### Updated Dependencies ####
- joda-time:joda-time:2.10.14
- org.apache.logging.log4j:log4j-api:2.17.2
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.15.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.15.1

### interlok-elastic-rest ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- joda-time:joda-time:2.10.14
- org.apache.logging.log4j:log4j-api:2.17.2
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-excel ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-exec ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-expressions ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-failover ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-filesystem ###

#### Updated Dependencies ####
- com.hierynomus:smbj:0.11.5
- org.apache.tika:tika-core:2.4.0
- org.json:json:20220320
- org.slf4j:slf4j-api:1.7.36

### interlok-flyway ###

#### Updated Dependencies ####
- org.flywaydb:flyway-core:8.5.11

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.google.cloud:google-cloud-pubsub:1.118.0
- com.google.code.gson:gson:2.9.0
- com.google.guava:guava:31.1-jre
- com.google.protobuf:protobuf-java-util:3.20.1
- com.google.protobuf:protobuf-java:3.20.1
- io.grpc:grpc-alts:1.46.0
- io.grpc:grpc-auth:1.46.0
- io.grpc:grpc-netty:1.46.0
- io.grpc:grpc-protobuf:1.46.0
- io.grpc:grpc-stub:1.46.0
- io.netty:netty-codec-http2:4.1.77.Final
- io.netty:netty-codec-http:4.1.77.Final
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-handler-proxy:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-hpcc ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-jclouds-aws-sts ###

#### Updated Dependencies ####
- org.apache.jclouds.api:sts:2.5.0
- org.slf4j:slf4j-api:1.7.36

### interlok-jclouds-blobstore ###

#### Updated Dependencies ####
- org.apache.jclouds:jclouds-blobstore:2.5.0
- org.slf4j:slf4j-api:1.7.36

### interlok-jclouds-common ###

#### Updated Dependencies ####
- com.google.guava:guava:31.1-jre
- org.apache.jclouds:jclouds-core:2.5.0
- org.slf4j:slf4j-api:1.7.36

### interlok-jdbc ###

#### Updated Dependencies ####
- com.google.guava:guava:31.1-jre
- org.slf4j:slf4j-api:1.7.36

### interlok-jms-oracleaq ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-jms-sonicmq ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-jmx-activemq ###

#### Updated Dependencies ####
- org.apache.activemq:activemq-client:5.17.1
- org.slf4j:slf4j-api:1.7.36
- org.springframework:spring-aop:5.3.20
- org.springframework:spring-beans:5.3.20
- org.springframework:spring-context:5.3.20
- org.springframework:spring-core:5.3.20
- org.springframework:spring-jms:5.3.20

### interlok-jmx-amqp ###

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.77.Final
- io.netty:netty-codec-http:4.1.77.Final
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-common:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final
- io.netty:netty-transport-native-kqueue:4.1.77.Final
- io.netty:netty-transport-native-unix-common:4.1.77.Final
- io.netty:netty-transport:4.1.77.Final
- org.apache.qpid:qpid-jms-client:1.6.0
- org.slf4j:slf4j-api:1.7.36
- org.springframework:spring-aop:5.3.20
- org.springframework:spring-beans:5.3.20
- org.springframework:spring-context:5.3.20
- org.springframework:spring-core:5.3.20
- org.springframework:spring-jms:5.3.20

### interlok-jmx-jms-common ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36
- org.springframework:spring-aop:5.3.20
- org.springframework:spring-beans:5.3.20
- org.springframework:spring-context:5.3.20
- org.springframework:spring-core:5.3.20
- org.springframework:spring-jms:5.3.20

### interlok-jmx-jms-stubs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- org.apache.activemq:activemq-amqp:5.17.1
- org.apache.activemq:activemq-broker:5.17.1
- org.apache.activemq:activemq-jaas:5.17.1
- org.apache.activemq:activemq-kahadb-store:5.17.1
- org.slf4j:slf4j-api:1.7.36
- org.springframework:spring-aop:5.3.20
- org.springframework:spring-beans:5.3.20
- org.springframework:spring-context:5.3.20
- org.springframework:spring-core:5.3.20
- org.springframework:spring-jms:5.3.20

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-jmx-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.14.0
- com.solacesystems:sol-jcsmp:10.14.0
- com.solacesystems:sol-jms:10.14.0
- org.slf4j:slf4j-api:1.7.36
- org.springframework:spring-aop:5.3.20
- org.springframework:spring-beans:5.3.20
- org.springframework:spring-context:5.3.20
- org.springframework:spring-core:5.3.20
- org.springframework:spring-jms:5.3.20

### interlok-jmx-sonicmq ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-jolokia ###

#### Updated Dependencies ####
- org.eclipse.jetty.aggregate:jetty-all:9.4.46.v20220331

### interlok-jq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-jruby ###

#### Updated Dependencies ####
- org.jruby:jruby:9.3.4.0
- org.slf4j:slf4j-api:1.7.36

### interlok-jslt ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.schibsted.spt.data:jslt:0.1.12
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:
- com.fasterxml.jackson:jackson-bom:2.13.3
- com.github.erosb:everit-json-schema:1.14.1

#### Updated Dependencies ####
- com.bazaarvoice.jolt:jolt-core:0.1.7
- com.bazaarvoice.jolt:json-utils:0.1.7
- com.flipkart.zjsonpatch:zjsonpatch:0.4.12
- com.google.guava:guava:31.1-jre
- org.json:json:20220320
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.13.1
- com.github.everit-org.json-schema:org.everit.json.schema:1.14.0

### interlok-json-streaming ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.google.code.gson:gson:2.9.0
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-json-web-token ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- io.jsonwebtoken:jjwt-api:0.11.5
- io.jsonwebtoken:jjwt-impl:0.11.5
- io.jsonwebtoken:jjwt-jackson:0.11.5
- org.json:json:20220320
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.5

### interlok-jsr107-cache ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-kafka ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3
- org.apache.zookeeper:zookeeper:3.8.0

#### Updated Dependencies ####
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-kie ###

#### Updated Dependencies ####
- org.drools:drools-compiler:7.70.0.Final
- org.drools:drools-core:7.70.0.Final
- org.slf4j:slf4j-api:1.7.36

### interlok-licensing ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-licensing-demo ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-logging ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-api:2.17.2
- org.apache.logging.log4j:log4j-core:2.17.2

### interlok-mongodb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- org.mongodb:mongodb-driver:3.12.11
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-mqtt ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-msmq-javonet ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-nats ###

#### Updated Dependencies ####
- io.nats:jnats:2.15.1

### interlok-oauth-azure ###

#### New Dependencies ####
- com.google.code.gson:gson:2.9.0

#### Updated Dependencies ####
- com.nimbusds:nimbus-jose-jwt:9.22
- net.minidev:json-smart:2.4.8
- org.slf4j:slf4j-api:1.7.36

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.3
- com.google.auth:google-auth-library-oauth2-http:1.7.0
- com.google.guava:guava:31.1-jre
- org.slf4j:slf4j-api:1.7.36

### interlok-oauth-generic ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-oauth-salesforce ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-okhttp ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-pdf ###

#### Updated Dependencies ####
- com.google.guava:guava:31.1-jre
- org.apache.pdfbox:fontbox:2.0.26
- org.apache.pdfbox:pdfbox-tools:2.0.26
- org.apache.pdfbox:pdfbox:2.0.26
- org.slf4j:slf4j-api:1.7.36

### interlok-pgp ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-profiler ###

#### Updated Dependencies ####
- org.aspectj:aspectjrt:1.9.9.1
- org.aspectj:aspectjtools:1.9.9.1
- org.aspectj:aspectjweaver:1.9.9.1
- org.slf4j:slf4j-api:1.7.36

### interlok-proxy ###

#### Updated Dependencies ####
- org.apache.httpcomponents.client5:httpclient5:5.1.3

### interlok-rabbitmq ###

#### Updated Dependencies ####
- com.rabbitmq:amqp-client:5.14.2
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-rest-metrics-jvm ###

#### Updated Dependencies ####
- io.micrometer:micrometer-core:1.9.0

### interlok-rest-provider-datadog ###

#### Updated Dependencies ####
- io.micrometer:micrometer-registry-datadog:1.9.0

### interlok-rest-provider-prometheus ###

#### Updated Dependencies ####
- io.micrometer:micrometer-registry-prometheus:1.9.0

### interlok-sap ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-service-tester ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-service-tester-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- org.json:json:20220320
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-service-tester-wiremock ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.github.tomakehurst:wiremock-jre8:2.33.2
- com.google.guava:guava:31.1-jre
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-service-tester-xml ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.14.0
- com.solacesystems:sol-jcsmp:10.14.0
- com.solacesystems:sol-jms:10.14.0
- org.slf4j:slf4j-api:1.7.36

### interlok-sshtunnel ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.2.1
- org.slf4j:slf4j-api:1.7.36

### interlok-stax ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-stubs ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-swift ###

#### Updated Dependencies ####
- com.prowidesoftware:pw-swift-core:SRU2021-9.2.13
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-tibco ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-triggered ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-vcs-git ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.2.1
- org.slf4j:slf4j-api:1.7.36

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- org.apache.cxf:cxf-rt-frontend-jaxws:3.5.2
- org.apache.cxf:cxf-rt-transports-http:3.5.2
- org.slf4j:slf4j-api:1.7.36

### interlok-webspheremq ###

#### Updated Dependencies ####
- com.ibm.mq:com.ibm.mq.allclient:9.2.5.0
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-work-unit ###

#### Initial Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-activemq ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-atomikos ###

#### Updated Dependencies ####
- org.awaitility:awaitility:4.2.0
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-jms ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.14.0
- com.solacesystems:sol-jcsmp:10.14.0
- com.solacesystems:sol-jms:10.14.0
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-tibco ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-wmq ###

#### Updated Dependencies ####
- com.ibm.mq:com.ibm.mq.allclient:9.2.5.0
- org.slf4j:slf4j-api:1.7.36

### interlok-xml-security ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36
