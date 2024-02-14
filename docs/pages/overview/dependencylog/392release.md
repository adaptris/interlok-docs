## Version 3.9.2-RELEASE ##

### interlok-actional-interceptor ###

#### New Dependencies ####
- org.slf4j:slf4j-log4j12:1.7.28

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

#### Removed Dependencies ####
- org.apache.velocity:velocity:1.7

### interlok-actional-stabiliser ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28
- org.slf4j:slf4j-log4j12:1.7.28

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7

### interlok-activemq ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.10.0
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- com.google.guava:guava:28.1-jre
- org.apache.activemq:activemq-amqp:5.15.10
- org.apache.activemq:activemq-broker:5.15.10
- org.apache.activemq:activemq-client:5.15.10
- org.apache.activemq:activemq-jaas:5.15.10
- org.apache.activemq:activemq-kahadb-store:5.15.10
- org.apache.activemq:activemq-mqtt:5.15.10
- org.apache.activemq:activemq-spring:5.15.10
- org.apache.activemq:activemq-stomp:5.15.10
- org.apache.qpid:proton-j:0.33.2

### interlok-amqp ###

#### Updated Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:1.13.0
- org.apache.qpid:proton-j:0.33.2
- org.apache.qpid:qpid-jms-client:0.46.0
- org.slf4j:slf4j-api:1.7.28

### interlok-apache-http ###

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.10

### interlok-artemis ###

#### Updated Dependencies ####
- org.apache.activemq:artemis-jms-server:2.10.1

### interlok-aws-common ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.646
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

### interlok-aws-kinesis ###

#### Updated Dependencies ####
- com.amazonaws:amazon-kinesis-client:1.11.2
- com.amazonaws:aws-java-sdk-kinesis:1.11.646
- com.fasterxml.jackson.core:jackson-core:2.10.0
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- com.google.protobuf:protobuf-java:3.10.0
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

### interlok-aws-s3 ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.646
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

### interlok-aws-sns ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.646
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

### interlok-aws-sqs ###

#### Updated Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.0.8
- com.amazonaws:aws-java-sdk-sqs:1.11.646
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- org.apache.httpcomponents:httpclient:4.5.10
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

### interlok-azure-cosmosdb ###

#### Initial Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.10.0
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- com.microsoft.azure:azure-documentdb:2.4.2
- org.slf4j:slf4j-api:1.7.28

### interlok-cassandra ###

#### Updated Dependencies ####
- com.google.guava:guava:28.1-jre
- org.slf4j:slf4j-api:1.7.28

### interlok-client ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-client-jmx ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-cluster-manager ###

#### Updated Dependencies ####
- org.jgroups:jgroups:4.1.5.Final

### interlok-common ###

#### New Dependencies ####
- org.mockito:mockito-all:1.10.19

#### Updated Dependencies ####
- javax.servlet:javax.servlet-api:4.0.1
- org.eclipse.jetty.aggregate:jetty-all:9.4.20.v20190813

### interlok-config-conditional ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-core ###

#### New Dependencies ####
- com.zaxxer:HikariCP:3.4.1
- org.glassfish:javax.el:3.0.1-b11
- org.hibernate.validator:hibernate-validator:6.0.17.Final

#### Updated Dependencies ####
- javax.servlet:javax.servlet-api:4.0.1
- javax.validation:validation-api:2.0.1.Final
- org.apache.activemq:activemq-broker:5.15.10
- org.apache.activemq:activemq-client:5.15.10
- org.apache.activemq:activemq-jaas:5.15.10
- org.apache.activemq:activemq-kahadb-store:5.15.10
- org.apache.activemq:artemis-jms-server:2.10.1
- org.apache.commons:commons-text:1.8
- org.bouncycastle:bcmail-jdk15on:1.64
- org.bouncycastle:bcpkix-jdk15on:1.64
- org.bouncycastle:bcprov-jdk15on:1.64
- org.eclipse.jetty.aggregate:jetty-all:9.4.20.v20190813
- org.jruby:jruby-complete:9.2.8.0

#### Removed Dependencies ####
- commons-pool:commons-pool:1.6
- javax.el:javax.el-api:2.2.4
- org.hibernate:hibernate-validator:4.3.2.Final

### interlok-core-apt ###

#### New Dependencies ####
- org.glassfish:javax.el:3.0.1-b11
- org.hibernate.validator:hibernate-validator:6.0.17.Final

#### Updated Dependencies ####
- javax.validation:validation-api:2.0.1.Final

#### Removed Dependencies ####
- org.hibernate:hibernate-validator:4.3.2.Final

### interlok-csv ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-csv-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- org.slf4j:slf4j-api:1.7.28

### interlok-drools ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-ehcache ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-elastic-common ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- joda-time:joda-time:2.10.4
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.3.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.3.1
- org.slf4j:slf4j-api:1.7.28

### interlok-elastic-rest ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- joda-time:joda-time:2.10.4
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.3.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.3.1
- org.slf4j:slf4j-api:1.7.28

### interlok-elastic-search ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-es-rest ###

#### Updated Dependencies ####
- joda-time:joda-time:2.10.4
- org.slf4j:slf4j-api:1.7.28

### interlok-es5 ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- org.slf4j:slf4j-api:1.7.28

### interlok-excel ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-exec ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-expressions ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-filesystem ###

#### Updated Dependencies ####
- org.apache.commons:commons-compress:1.19
- org.slf4j:slf4j-api:1.7.28

### interlok-flyway ###

#### Updated Dependencies ####
- org.flywaydb:flyway-core:6.0.6

### interlok-gcloud-pubsub ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- com.google.cloud:google-cloud-pubsub:1.92.0
- com.google.guava:guava:28.1-jre
- org.apache.httpcomponents:httpclient:4.5.10

### interlok-hpcc ###

#### New Dependencies ####
- oro:oro:2.0.8

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-ironmq ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

#### Removed Dependencies ####
- org.quartz-scheduler:quartz:2.2.1

### interlok-jclouds-blobstore ###

#### Updated Dependencies ####
- com.google.guava:guava:28.1-jre
- org.slf4j:slf4j-api:1.7.28

### interlok-jms-oracleaq ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

### interlok-jq ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- org.slf4j:slf4j-api:1.7.28

### interlok-jruby ###

#### Updated Dependencies ####
- org.jruby:jruby:9.2.8.0
- org.slf4j:slf4j-api:1.7.28

### interlok-json ###

#### New Dependencies ####
- com.github.everit-org.json-schema:org.everit.json.schema:1.12.0

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.10.0
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.10.0
- com.google.guava:guava:28.1-jre
- org.slf4j:slf4j-api:1.7.28

#### Removed Dependencies ####
- org.everit.json:org.everit.json.schema:1.5.1

### interlok-jsr107-cache ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-kafka ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- org.slf4j:slf4j-api:1.7.28

### interlok-kie ###

#### Updated Dependencies ####
- org.drools:drools-compiler:7.27.0.Final
- org.drools:drools-core:7.27.0.Final
- org.slf4j:slf4j-api:1.7.28

### interlok-kubernetes-metrics ###

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

### interlok-kubernetes-prometheus ###

#### Updated Dependencies ####
- io.prometheus:simpleclient:0.7.0
- io.prometheus:simpleclient_hotspot:0.7.0
- io.prometheus:simpleclient_httpserver:0.7.0
- io.prometheus:simpleclient_pushgateway:0.7.0
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

### interlok-legacyhttp ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-mongodb ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- org.mongodb:mongodb-driver:3.11.0
- org.slf4j:slf4j-api:1.7.28

### interlok-monitor-agent ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-mqtt ###

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.10
- org.eclipse.paho:org.eclipse.paho.client.mqttv3:1.2.2
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28
- org.slf4j:slf4j-log4j12:1.7.28

### interlok-oauth-azure ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.10.0
- com.google.auth:google-auth-library-oauth2-http:0.17.2
- com.google.guava:guava:28.1-jre
- org.apache.httpcomponents:httpclient:4.5.10
- org.slf4j:slf4j-api:1.7.28

### interlok-oauth-generic ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- org.slf4j:slf4j-api:1.7.28

### interlok-oauth-salesforce ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- org.apache.httpcomponents:httpclient:4.5.10
- org.slf4j:slf4j-api:1.7.28

### interlok-okhttp ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-pdf ###

#### Updated Dependencies ####
- com.google.guava:guava:28.1-jre
- org.apache.pdfbox:fontbox:2.0.17
- org.apache.pdfbox:pdfbox-tools:2.0.17
- org.apache.pdfbox:pdfbox:2.0.17
- org.slf4j:slf4j-api:1.7.28

### interlok-pgp ###

#### Initial Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.64
- org.bouncycastle:bcprov-jdk15on:1.64
- org.slf4j:slf4j-api:1.7.28

### interlok-profiler ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-service-tester ###

#### Updated Dependencies ####
- com.github.tomakehurst:wiremock:2.25.0
- org.apache.ant:ant-junit:1.10.7
- org.slf4j:slf4j-api:1.7.28

### interlok-shell ###

#### Updated Dependencies ####
- org.bouncycastle:bcpkix-jdk15on:1.64
- org.bouncycastle:bcprov-jdk15on:1.64
- org.slf4j:slf4j-api:1.7.28

### interlok-socket ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-sshtunnel ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-stax ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-stubs ###

#### New Dependencies ####
- com.zaxxer:HikariCP:3.4.1
- org.glassfish:javax.el:3.0.1-b11
- org.hibernate.validator:hibernate-validator:6.0.17.Final

#### Updated Dependencies ####
- javax.servlet:javax.servlet-api:4.0.1
- javax.validation:validation-api:2.0.1.Final
- org.apache.activemq:activemq-broker:5.15.10
- org.apache.activemq:activemq-client:5.15.10
- org.apache.activemq:activemq-jaas:5.15.10
- org.apache.activemq:activemq-kahadb-store:5.15.10
- org.apache.activemq:artemis-jms-server:2.10.1
- org.apache.commons:commons-text:1.8
- org.bouncycastle:bcmail-jdk15on:1.64
- org.bouncycastle:bcpkix-jdk15on:1.64
- org.bouncycastle:bcprov-jdk15on:1.64
- org.eclipse.jetty.aggregate:jetty-all:9.4.20.v20190813
- org.jruby:jruby-complete:9.2.8.0

#### Removed Dependencies ####
- commons-pool:commons-pool:1.6
- javax.el:javax.el-api:2.2.4
- org.hibernate:hibernate-validator:4.3.2.Final

### interlok-swift ###

#### New Dependencies ####
- com.prowidesoftware:pw-swift-core:SRU2018-7.10.4

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.28
- org.slf4j:slf4j-api:1.7.28

#### Removed Dependencies ####
- com.prowidesoftware.swift:swift:7.0

### interlok-vcs-command-line ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.28

### interlok-vcs-git ###

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.10
- org.eclipse.jgit:org.eclipse.jgit:5.5.0.201909110433-r
- org.slf4j:slf4j-api:1.7.28

### interlok-vertx ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.10.0
- com.hazelcast:hazelcast:3.12.3
- io.vertx:vertx-core:3.8.2
- io.vertx:vertx-hazelcast:3.8.2
- org.slf4j:slf4j-api:1.7.28

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- org.apache.cxf:cxf-rt-frontend-jaxws:3.3.3
- org.apache.cxf:cxf-rt-transports-http:3.3.3
- org.slf4j:slf4j-api:1.7.28

### interlok-xa-atomikos ###

#### New Dependencies ####
- org.awaitility:awaitility:4.0.1
