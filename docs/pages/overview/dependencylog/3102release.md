## Version 3.10.2-RELEASE ##

### interlok-activemq ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.11.0
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- org.apache.qpid:proton-j:0.33.5
- org.springframework:spring-beans:4.3.27.RELEASE
- org.springframework:spring-context:4.3.27.RELEASE

### interlok-amqp ###

#### Updated Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:2.1.1
- io.netty:netty-buffer:4.1.50.Final
- io.netty:netty-codec-http:4.1.50.Final
- io.netty:netty-codec:4.1.50.Final
- io.netty:netty-common:4.1.50.Final
- io.netty:netty-handler:4.1.50.Final
- io.netty:netty-transport-native-epoll:4.1.50.Final
- io.netty:netty-transport-native-kqueue:4.1.50.Final
- io.netty:netty-transport-native-unix-common:4.1.50.Final
- io.netty:netty-transport:4.1.50.Final
- org.apache.qpid:proton-j:0.33.5
- org.apache.qpid:qpid-client:6.4.0
- org.apache.qpid:qpid-jms-client:0.52.0

### interlok-apache-geode ###

#### New Dependencies ####
- commons-beanutils:commons-beanutils:1.9.4

### interlok-apache-http ###

#### New Dependencies ####
- commons-codec:commons-codec:1.14

### interlok-artemis ###

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.50.Final
- io.netty:netty-codec-http:4.1.50.Final
- io.netty:netty-codec:4.1.50.Final
- io.netty:netty-common:4.1.50.Final
- io.netty:netty-handler:4.1.50.Final
- io.netty:netty-transport-native-epoll:4.1.50.Final
- io.netty:netty-transport-native-kqueue:4.1.50.Final
- io.netty:netty-transport-native-unix-common:4.1.50.Final
- io.netty:netty-transport:4.1.50.Final
- org.apache.activemq:artemis-jms-server:2.12.0
- org.apache.activemq:artemis-server:2.12.0

### interlok-aws-common ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.11.0
- com.fasterxml.jackson.core:jackson-core:2.11.0
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.11.0

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.803

### interlok-aws-kinesis ###

#### New Dependencies ####
- commons-codec:commons-codec:1.14

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-kinesis:1.11.803
- com.fasterxml.jackson.core:jackson-core:2.11.0
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- com.google.protobuf:protobuf-java:3.12.2

### interlok-aws-kms ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-kms:1.11.803

### interlok-aws-s3 ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.803

### interlok-aws-sns ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.803

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.803

### interlok-aws-sqs ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.803
- commons-codec:commons-codec:1.14

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sqs:1.11.803
- com.fasterxml.jackson.core:jackson-databind:2.11.0

### interlok-azure-cosmosdb ###

#### New Dependencies ####
- commons-codec:commons-codec:1.14

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.11.0
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- com.microsoft.azure:azure-documentdb:2.5.1

### interlok-cassandra ###

#### New Dependencies ####
- io.netty:netty-codec:4.1.50.Final
- io.netty:netty-handler:4.1.50.Final
- io.netty:netty-transport-native-epoll:4.1.50.Final

#### Updated Dependencies ####
- com.datastax.cassandra:cassandra-driver-core:3.9.0
- com.datastax.cassandra:cassandra-driver-mapping:3.9.0
- com.fasterxml.jackson.core:jackson-core:2.11.0
- com.fasterxml.jackson.core:jackson-databind:2.11.0

### interlok-client ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-1.2-api:2.13.3
- org.apache.logging.log4j:log4j-api:2.13.3
- org.apache.logging.log4j:log4j-core:2.13.3

### interlok-client-jmx ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-1.2-api:2.13.3
- org.apache.logging.log4j:log4j-api:2.13.3
- org.apache.logging.log4j:log4j-core:2.13.3

### interlok-cluster-manager ###

#### Updated Dependencies ####
- org.jgroups:jgroups:4.2.4.Final

### interlok-common ###

#### New Dependencies ####
- org.apache.logging.log4j:log4j-1.2-api:2.13.3
- org.apache.logging.log4j:log4j-api:2.13.3
- org.apache.logging.log4j:log4j-core:2.13.3
- org.apache.logging.log4j:log4j-slf4j-impl:2.13.3
- org.slf4j:jcl-over-slf4j:1.7.30
- org.slf4j:jul-to-slf4j:1.7.30

#### Updated Dependencies ####
- commons-io:commons-io:2.7
- org.eclipse.jetty.aggregate:jetty-all:9.4.30.v20200611

### interlok-core ###

#### Updated Dependencies ####
- com.zaxxer:HikariCP:3.4.5
- commons-io:commons-io:2.7
- org.apache.activemq:artemis-jms-server:2.12.0
- org.awaitility:awaitility:4.0.3
- org.eclipse.jetty.aggregate:jetty-all:9.4.30.v20200611
- org.hibernate.validator:hibernate-validator:6.1.5.Final

#### Removed Dependencies ####
- org.apache.logging.log4j:log4j-1.2-api:2.13.2
- org.apache.logging.log4j:log4j-api:2.13.2
- org.apache.logging.log4j:log4j-core:2.13.2
- org.apache.logging.log4j:log4j-slf4j-impl:2.13.2
- org.slf4j:jcl-over-slf4j:1.7.30
- org.slf4j:jul-to-slf4j:1.7.30

### interlok-core-apt ###

#### Updated Dependencies ####
- org.hibernate.validator:hibernate-validator:6.1.5.Final

### interlok-csv-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0

### interlok-drools ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.12

### interlok-elastic-common ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- commons-codec:commons-codec:1.14
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.7.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.7.1

### interlok-elastic-rest ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- commons-codec:commons-codec:1.14
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.7.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.7.1

### interlok-es-rest ###

#### Updated Dependencies ####
- org.json:json:20200518

### interlok-es5 ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0

### interlok-excel ###

#### Updated Dependencies ####
- org.apache.poi:poi-ooxml:4.1.2
- org.apache.poi:poi:4.1.2

### interlok-filesystem ###

#### Updated Dependencies ####
- org.json:json:20200518

### interlok-flyway ###

#### Updated Dependencies ####
- org.flywaydb:flyway-core:6.4.4

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.google.code.gson:gson:2.8.6
- com.google.protobuf:protobuf-java-util:3.12.2
- com.google.protobuf:protobuf-java:3.12.2
- commons-codec:commons-codec:1.14
- io.grpc:grpc-alts:1.30.1
- io.grpc:grpc-auth:1.30.1
- io.grpc:grpc-netty:1.30.1
- io.grpc:grpc-protobuf:1.30.1
- io.grpc:grpc-stub:1.30.1
- io.netty:netty-codec:4.1.50.Final
- io.netty:netty-handler:4.1.50.Final
- io.netty:netty-transport-native-epoll:4.1.50.Final

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- com.google.cloud:google-cloud-pubsub:1.107.0

### interlok-jclouds-aws-sts ###

#### Initial Dependencies ####
- org.apache.jclouds.api:sts:2.2.1
- org.slf4j:slf4j-api:1.7.30

### interlok-jclouds-blobstore ###

#### Updated Dependencies ####
- org.apache.jclouds:jclouds-blobstore:2.2.1

#### Removed Dependencies ####
- com.google.guava:guava:29.0-jre

### interlok-jclouds-common ###

#### Initial Dependencies ####
- com.google.guava:guava:29.0-jre
- org.apache.jclouds:jclouds-core:2.2.1
- org.slf4j:slf4j-api:1.7.30

### interlok-jmx-activemq ###

#### Updated Dependencies ####
- org.springframework:spring-aop:4.3.27.RELEASE
- org.springframework:spring-beans:4.3.27.RELEASE
- org.springframework:spring-context:4.3.27.RELEASE
- org.springframework:spring-core:4.3.27.RELEASE
- org.springframework:spring-jms:4.3.27.RELEASE

### interlok-jmx-amqp ###

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.50.Final
- io.netty:netty-codec-http:4.1.50.Final
- io.netty:netty-codec:4.1.50.Final
- io.netty:netty-common:4.1.50.Final
- io.netty:netty-handler:4.1.50.Final
- io.netty:netty-transport-native-epoll:4.1.50.Final
- io.netty:netty-transport-native-kqueue:4.1.50.Final
- io.netty:netty-transport-native-unix-common:4.1.50.Final
- io.netty:netty-transport:4.1.50.Final
- org.apache.qpid:proton-j:0.33.5
- org.apache.qpid:qpid-jms-client:0.52.0
- org.springframework:spring-aop:4.3.27.RELEASE
- org.springframework:spring-beans:4.3.27.RELEASE
- org.springframework:spring-context:4.3.27.RELEASE
- org.springframework:spring-core:4.3.27.RELEASE
- org.springframework:spring-jms:4.3.27.RELEASE

### interlok-jmx-jms-common ###

#### Updated Dependencies ####
- org.springframework:spring-aop:4.3.27.RELEASE
- org.springframework:spring-beans:4.3.27.RELEASE
- org.springframework:spring-context:4.3.27.RELEASE
- org.springframework:spring-core:4.3.27.RELEASE
- org.springframework:spring-jms:4.3.27.RELEASE

### interlok-jmx-jms-stubs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.11.0
- com.fasterxml.jackson.core:jackson-databind:2.11.0

#### Updated Dependencies ####
- commons-io:commons-io:2.7
- org.springframework:spring-aop:4.3.27.RELEASE
- org.springframework:spring-beans:4.3.27.RELEASE
- org.springframework:spring-context:4.3.27.RELEASE
- org.springframework:spring-core:4.3.27.RELEASE
- org.springframework:spring-jms:4.3.27.RELEASE

### interlok-jmx-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.9.0
- com.solacesystems:sol-jcsmp:10.9.0
- com.solacesystems:sol-jms:10.9.0
- org.springframework:spring-aop:4.3.27.RELEASE
- org.springframework:spring-beans:4.3.27.RELEASE
- org.springframework:spring-context:4.3.27.RELEASE
- org.springframework:spring-core:4.3.27.RELEASE
- org.springframework:spring-jms:4.3.27.RELEASE

### interlok-jq ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0

### interlok-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.11.0
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.11.0
- org.json:json:20200518
- xom:xom:1.3.5

### interlok-kafka ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- io.netty:netty-codec:4.1.50.Final
- io.netty:netty-handler:4.1.50.Final
- io.netty:netty-transport-native-epoll:4.1.50.Final

### interlok-kie ###

#### New Dependencies ####
- commons-codec:commons-codec:1.14

#### Updated Dependencies ####
- org.drools:drools-compiler:7.38.0.Final
- org.drools:drools-core:7.38.0.Final

### interlok-kubernetes-prometheus ###

#### Updated Dependencies ####
- io.prometheus:simpleclient:0.9.0
- io.prometheus:simpleclient_hotspot:0.9.0
- io.prometheus:simpleclient_httpserver:0.9.0
- io.prometheus:simpleclient_pushgateway:0.9.0

### interlok-logging ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-api:2.13.3
- org.apache.logging.log4j:log4j-core:2.13.3

### interlok-mongodb ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- org.mongodb:mongodb-driver:3.12.5

### interlok-mqtt ###

#### New Dependencies ####
- commons-codec:commons-codec:1.14

#### Removed Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.30
- org.slf4j:slf4j-log4j12:1.7.30

### interlok-nats ###

#### Updated Dependencies ####
- io.nats:jnats:2.6.8

### interlok-oauth-gcloud ###

#### New Dependencies ####
- commons-codec:commons-codec:1.14

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.11.0

### interlok-oauth-generic ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0

### interlok-oauth-salesforce ###

#### New Dependencies ####
- commons-codec:commons-codec:1.14

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0

### interlok-okhttp ###

#### Updated Dependencies ####
- com.squareup.okhttp3:okhttp:4.7.2

### interlok-pdf ###

#### Updated Dependencies ####
- org.apache.pdfbox:fontbox:2.0.20
- org.apache.pdfbox:pdfbox-tools:2.0.20
- org.apache.pdfbox:pdfbox:2.0.20
- org.apache.xmlgraphics:fop:2.5

### interlok-profiler-metric-services ###

#### Updated Dependencies ####
- org.codehaus.groovy:groovy-json:2.5.12
- org.codehaus.groovy:groovy:2.5.12

### interlok-profiler-prometheus ###

#### Updated Dependencies ####
- io.prometheus:simpleclient:0.9.0
- io.prometheus:simpleclient_hotspot:0.9.0
- io.prometheus:simpleclient_httpserver:0.9.0
- io.prometheus:simpleclient_pushgateway:0.9.0

#### Removed Dependencies ####
- com.pivovarit:throwing-function:1.5.0

### interlok-service-tester-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.11.0
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- org.json:json:20200518

### interlok-service-tester-wiremock ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.11.0
- com.fasterxml.jackson.core:jackson-core:2.11.0
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- com.google.guava:guava:29.0-jre

### interlok-shell ###

#### Updated Dependencies ####
- org.codehaus.groovy:groovy-all:2.5.12

### interlok-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.9.0
- com.solacesystems:sol-jcsmp:10.9.0
- com.solacesystems:sol-jms:10.9.0

### interlok-stubs ###

#### Updated Dependencies ####
- com.zaxxer:HikariCP:3.4.5
- commons-io:commons-io:2.7
- org.apache.activemq:artemis-jms-server:2.12.0
- org.awaitility:awaitility:4.0.3
- org.eclipse.jetty.aggregate:jetty-all:9.4.30.v20200611
- org.hibernate.validator:hibernate-validator:6.1.5.Final

#### Removed Dependencies ####
- org.apache.logging.log4j:log4j-1.2-api:2.13.2
- org.apache.logging.log4j:log4j-api:2.13.2
- org.apache.logging.log4j:log4j-core:2.13.2
- org.apache.logging.log4j:log4j-slf4j-impl:2.13.2
- org.slf4j:jcl-over-slf4j:1.7.30
- org.slf4j:jul-to-slf4j:1.7.30

### interlok-vcs-git ###

#### New Dependencies ####
- commons-codec:commons-codec:1.14

### interlok-vertx ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.11.0
- io.vertx:vertx-core:3.9.1
- io.vertx:vertx-hazelcast:3.9.1

### interlok-xa-solace ###

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.9.0
- com.solacesystems:sol-jcsmp:10.9.0
- com.solacesystems:sol-jms:10.9.0
