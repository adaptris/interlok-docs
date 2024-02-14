## Version 3.8.1-RELEASE ##

### interlok-activemq ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.9.7
- com.fasterxml.jackson.core:jackson-databind:2.9.7
- org.apache.activemq:activemq-amqp:5.15.6
- org.apache.activemq:activemq-broker:5.15.6
- org.apache.activemq:activemq-client:5.15.6
- org.apache.activemq:activemq-jaas:5.15.6
- org.apache.activemq:activemq-kahadb-store:5.15.6
- org.apache.activemq:activemq-mqtt:5.15.6
- org.apache.activemq:activemq-spring:5.15.6
- org.apache.activemq:activemq-stomp:5.15.6
- org.springframework:spring-beans:4.3.19.RELEASE
- org.springframework:spring-context:4.3.19.RELEASE

### interlok-amqp ###

#### Updated Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:1.10.0
- com.rabbitmq:amqp-client:5.4.1
- org.apache.qpid:proton-j:0.29.0
- org.apache.qpid:qpid-client:6.3.3
- org.apache.qpid:qpid-jms-client:0.36.0

### interlok-as2 ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- javax.servlet:javax.servlet-api:3.1.0
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.derby:derby:10.8.2.2
- org.apache.velocity:velocity:1.7
- org.eclipse.jetty.aggregate:jetty-all:9.4.1.v20170120
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-aws-sqs ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.7

### interlok-cassandra ###

#### New Dependencies ####
- com.google.guava:guava:26.0-jre

#### Updated Dependencies ####
- com.datastax.cassandra:cassandra-driver-core:3.6.0
- com.datastax.cassandra:cassandra-driver-mapping:3.6.0

### interlok-common ###

#### New Dependencies ####
- org.apache.commons:commons-pool2:2.6.0

### interlok-core ###

#### New Dependencies ####
- io.github.classgraph:classgraph:4.1.5
- org.apache.commons:commons-pool2:2.6.0

#### Updated Dependencies ####
- org.apache.activemq:activemq-broker:5.15.6
- org.apache.activemq:activemq-client:5.15.6
- org.apache.activemq:activemq-jaas:5.15.6
- org.apache.activemq:activemq-kahadb-store:5.15.6

#### Removed Dependencies ####
- io.github.lukehutch:fast-classpath-scanner:2.9.4

### interlok-csv-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.7

### interlok-drools ###

#### New Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.10
- org.apache.poi:poi-ooxml:3.17
- org.apache.poi:poi:3.17

#### Updated Dependencies ####
- org.antlr:antlr-runtime:3.5.2
- org.antlr:antlr-runtime:3.5.2
- org.antlr:antlr:3.5.2
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-es-rest ###

#### Updated Dependencies ####
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:6.4.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:6.4.1
- org.json:json:20180813

#### Removed Dependencies ####
- org.apache.commons:commons-compress:1.17

### interlok-es5 ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.7

### interlok-excel ###

#### Updated Dependencies ####
- org.apache.poi:poi-ooxml:3.17
- org.apache.poi:poi:3.17
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- commons-io:commons-io:2.4
- commons-lang:commons-lang:2.6
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-expressions ###

#### Removed Dependencies ####
- org.apache.commons:commons-compress:1.17

### interlok-filesystem ###

#### Updated Dependencies ####
- org.apache.commons:commons-compress:1.18
- org.json:json:20180813

### interlok-gcloud-pubsub ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.7
- com.google.cloud:google-cloud-pubsub:1.44.0

### interlok-hornetq ###

#### Updated Dependencies ####
- org.hornetq:hornetq-commons:2.4.7.Final
- org.hornetq:hornetq-core-client:2.4.7.Final
- org.hornetq:hornetq-jms-client:2.4.7.Final
- org.hornetq:hornetq-jms-server:2.4.7.Final
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-jclouds-blobstore ###

#### Updated Dependencies ####
- org.apache.jclouds:jclouds-blobstore:2.1.1

### interlok-jmx-jms ###

#### Updated Dependencies ####
- org.springframework:spring-aop:4.3.19.RELEASE
- org.springframework:spring-beans:4.3.19.RELEASE
- org.springframework:spring-context:4.3.19.RELEASE
- org.springframework:spring-core:4.3.19.RELEASE
- org.springframework:spring-jms:4.3.19.RELEASE

### interlok-jq ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.7

### interlok-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.7
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.9.7
- org.json:json:20180813

### interlok-kafka ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.7

#### Updated Dependencies ####
- org.apache.kafka:kafka-clients:1.1.1
- org.apache.kafka:kafka_2.11:1.1.1
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-legacyhttp ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.24
- org.slf4j:slf4j-log4j12:1.7.24

### interlok-mongodb ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.7
- org.mongodb:mongodb-driver:3.8.2

### interlok-new-relic ###

#### Updated Dependencies ####
- com.newrelic.agent.java:newrelic-api:4.6.0
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-oauth-azure ###

#### Updated Dependencies ####
- com.microsoft.azure:adal4j:1.6.2

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.google.auth:google-auth-library-oauth2-http:0.11.0

### interlok-oauth-generic ###

#### Initial Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- com.jayway.jsonpath:json-path:2.4.0
- org.slf4j:slf4j-api:1.7.25

### interlok-pdf ###

#### New Dependencies ####
- org.apache.pdfbox:fontbox:2.0.11

#### Updated Dependencies ####
- org.apache.xmlgraphics:fop:2.3
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- commons-io:commons-io:1.3.1
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.avalon.framework:avalon-framework-impl:4.3.1
- org.apache.velocity:velocity:1.7
- org.apache.xmlgraphics:batik-anim:1.7
- org.apache.xmlgraphics:batik-awt-util:1.7
- org.apache.xmlgraphics:batik-bridge:1.7
- org.apache.xmlgraphics:batik-css:1.7
- org.apache.xmlgraphics:batik-dom:1.7
- org.apache.xmlgraphics:batik-ext:1.7
- org.apache.xmlgraphics:batik-extension:1.7
- org.apache.xmlgraphics:batik-gvt:1.7
- org.apache.xmlgraphics:batik-js:1.7
- org.apache.xmlgraphics:batik-parser:1.7
- org.apache.xmlgraphics:batik-script:1.7
- org.apache.xmlgraphics:batik-svg-dom:1.7
- org.apache.xmlgraphics:batik-svggen:1.7
- org.apache.xmlgraphics:batik-transcoder:1.7
- org.apache.xmlgraphics:batik-util:1.7
- org.apache.xmlgraphics:batik-xml:1.7
- org.apache.xmlgraphics:xmlgraphics-commons:1.5
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-profiler ###

#### Removed Dependencies ####
- junit:junit:4.12
- log4j:log4j:1.2.17
- org.slf4j:jcl-over-slf4j:1.7.25
- org.slf4j:slf4j-log4j12:1.7.25

### interlok-reliable-messaging ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.derby:derby:10.10.1.1
- org.apache.geronimo.specs:geronimo-servlet_3.0_spec:1.0
- org.apache.velocity:velocity:1.7
- org.eclipse.jetty.aggregate:jetty-all:8.1.14.v20131031
- org.quartz-scheduler:quartz:2.2.1
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-schema ###

#### New Dependencies ####
- io.github.classgraph:classgraph:4.1.5

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.10
- io.github.lukehutch:fast-classpath-scanner:2.9.4
- junit:junit:3.8.1
- log4j:log4j:1.2.17
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-service-tester ###

#### Updated Dependencies ####
- com.github.tomakehurst:wiremock:2.18.0

### interlok-shell ###

#### Updated Dependencies ####
- org.codehaus.groovy:groovy-all:2.5.2

### interlok-solace ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- commons-lang:commons-lang:2.6
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-triggered ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-vcs-command-line ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-vcs-git ###

#### Updated Dependencies ####
- org.eclipse.jgit:org.eclipse.jgit:5.1.1.201809181055-r

### interlok-vertx ###

#### Updated Dependencies ####
- com.hazelcast:hazelcast:3.10.5

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- org.apache.cxf:cxf-rt-frontend-jaxws:3.2.6
- org.apache.cxf:cxf-rt-transports-http:3.2.6
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-webspheremq ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- cglib:cglib-nodep:2.2.2
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.hamcrest:hamcrest-core:1.3
- org.jmock:jmock-junit4:2.6.0
- org.jmock:jmock-legacy:2.6.0
- org.jmock:jmock:2.6.0
- org.mockito:mockito-all:1.9.5
- org.objenesis:objenesis:2.0
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-xml-security ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12
