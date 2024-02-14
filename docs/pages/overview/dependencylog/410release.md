## Version 4.1.0-RELEASE ##

### interlok-activemq ###

#### Updated Dependencies ####
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

### interlok-amqp ###

#### Updated Dependencies ####
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

### interlok-apache-geode ###

#### New Dependencies ####
- commons-codec:commons-codec:1.15

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- org.apache.geode:geode-core:1.13.2

### interlok-apache-http ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.30

#### Removed Dependencies ####
- commons-codec:commons-codec:1.15
- org.apache.commons:commons-lang3:3.12.0

### interlok-apache-http5 ###

#### Initial Dependencies ####
- org.apache.httpcomponents.client5:httpclient5:5.1
- org.slf4j:slf4j-api:1.7.30

### interlok-artemis ###

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.65.Final
- io.netty:netty-codec-http:4.1.65.Final
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-common:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final
- io.netty:netty-transport-native-kqueue:4.1.65.Final
- io.netty:netty-transport-native-unix-common:4.1.65.Final
- io.netty:netty-transport:4.1.65.Final

### interlok-aws-common ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.amazonaws:aws-java-sdk-sts:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

### interlok-aws-kinesis ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3
- com.google.guava:guava:30.1.1-jre
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
- com.amazonaws:amazon-kinesis-client:1.14.3
- com.amazonaws:amazon-kinesis-producer:0.14.7
- com.amazonaws:aws-java-sdk-kinesis:1.11.1034
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.google.protobuf:protobuf-java:3.17.2

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
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-kms:1.11.1034

### interlok-aws-s3 ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.1034

### interlok-aws-sns ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.1034

### interlok-aws-sqs ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.1034
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.3

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sqs:1.11.1034
- com.fasterxml.jackson.core:jackson-databind:2.12.3

### interlok-azure-core ###

#### New Dependencies ####
- net.minidev:json-smart:2.3.1

#### Updated Dependencies ####
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

### interlok-azure-cosmosdb ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.microsoft.azure:azure-documentdb:2.6.3

### interlok-cassandra ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final

### interlok-client ###

#### Updated Dependencies ####
- org.mockito:mockito-core:3.11.1
- org.mockito:mockito-inline:3.11.1

### interlok-client-jmx ###

#### Updated Dependencies ####
- org.mockito:mockito-core:3.11.1
- org.mockito:mockito-inline:3.11.1

### interlok-common ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- commons-io:commons-io:2.10.0
- org.apache.commons:commons-pool2:2.10.0
- org.eclipse.jetty.aggregate:jetty-all:9.4.42.v20210604
- org.mockito:mockito-core:3.11.1
- org.mockito:mockito-inline:3.11.1

### interlok-core ###

#### Updated Dependencies ####
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

### interlok-core-apt ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17

### interlok-csv-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

### interlok-ehcache ###

#### Updated Dependencies ####
- net.sf.ehcache:ehcache:2.10.9.2

### interlok-elastic-common ###

#### New Dependencies ####
- net.sf.supercsv:super-csv:2.4.0

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.jayway.jsonpath:json-path:2.6.0

### interlok-elastic-rest ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.jayway.jsonpath:json-path:2.6.0

### interlok-filesystem ###

#### Updated Dependencies ####
- com.hierynomus:smbj:0.11.1
- org.apache.tika:tika-core:1.26

### interlok-flyway ###

#### Updated Dependencies ####
- org.flywaydb:flyway-core:7.9.2

### interlok-gcloud-pubsub ###

#### Updated Dependencies ####
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

### interlok-jdbc ###

#### Initial Dependencies ####
- com.google.guava:guava:30.1.1-jre
- commons-codec:commons-codec:1.15
- org.codehaus.staxmate:stax2:2.1
- org.slf4j:slf4j-api:1.7.30

### interlok-jmx-activemq ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- org.apache.activemq:activemq-client:5.16.2
- org.springframework:spring-aop:5.3.7
- org.springframework:spring-beans:5.3.7
- org.springframework:spring-context:5.3.7
- org.springframework:spring-core:5.3.7
- org.springframework:spring-jms:5.3.7

### interlok-jmx-amqp ###

#### Updated Dependencies ####
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

### interlok-jmx-jms-common ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- org.springframework:spring-aop:5.3.7
- org.springframework:spring-beans:5.3.7
- org.springframework:spring-context:5.3.7
- org.springframework:spring-core:5.3.7
- org.springframework:spring-jms:5.3.7

### interlok-jmx-jms-stubs ###

#### Updated Dependencies ####
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

### interlok-jmx-solace ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- org.springframework:spring-aop:5.3.7
- org.springframework:spring-beans:5.3.7
- org.springframework:spring-context:5.3.7
- org.springframework:spring-core:5.3.7
- org.springframework:spring-jms:5.3.7

### interlok-jq ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

### interlok-jruby ###

#### Updated Dependencies ####
- org.jruby:jruby:9.2.17.0

### interlok-jslt ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

### interlok-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.12.3
- com.github.everit-org.json-schema:org.everit.json.schema:1.12.2
- com.jayway.jsonpath:json-path:2.6.0
- xom:xom:1.3.7

### interlok-json-streaming ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.github.jsurfer:jsurfer-gson:1.6.0
- com.github.jsurfer:jsurfer-jackson:1.6.0
- com.github.jsurfer:jsurfer-jsonsimple:1.6.0

### interlok-json-web-token ###

#### Updated Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.69
- org.bouncycastle:bcprov-jdk15on:1.69

### interlok-kafka ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- io.netty:netty-codec:4.1.65.Final
- io.netty:netty-handler:4.1.65.Final
- io.netty:netty-transport-native-epoll:4.1.65.Final

### interlok-kie ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.17
- org.drools:drools-compiler:7.54.0.Final
- org.drools:drools-core:7.54.0.Final

### interlok-mail ###

#### Updated Dependencies ####
- com.sun.mail:jakarta.mail:1.6.7

### interlok-mongodb ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

### interlok-nats ###

#### Updated Dependencies ####
- io.nats:jnats:2.11.4

### interlok-oauth-azure ###

#### Updated Dependencies ####
- com.microsoft.azure:adal4j:1.6.7
- net.minidev:json-smart:2.4.7

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.google.auth:google-auth-library-oauth2-http:0.26.0

### interlok-oauth-generic ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.jayway.jsonpath:json-path:2.6.0

### interlok-oauth-salesforce ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.3

### interlok-pdf ###

#### New Dependencies ####
- commons-io:commons-io:2.10.0

#### Updated Dependencies ####
- org.apache.pdfbox:fontbox:2.0.24
- org.apache.pdfbox:pdfbox-tools:2.0.24
- org.apache.pdfbox:pdfbox:2.0.24

### interlok-pgp ###

#### Updated Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.69
- org.bouncycastle:bcprov-jdk15on:1.69

### interlok-profiler ###

#### New Dependencies ####
- org.apache.commons:commons-math3:3.6.1

### interlok-rest-metrics-jvm ###

#### New Dependencies ####
- io.micrometer:micrometer-core:1.7.0

#### Removed Dependencies ####
- io.micrometer:micrometer-registry-prometheus:1.6.4

### interlok-rest-metrics-profiler ###

#### Removed Dependencies ####
- io.micrometer:micrometer-registry-prometheus:1.6.4

### interlok-rest-provider-datadog ###

#### Initial Dependencies ####
- io.micrometer:micrometer-registry-datadog:1.7.0

### interlok-rest-provider-prometheus ###

#### Updated Dependencies ####
- io.micrometer:micrometer-registry-prometheus:1.7.0

### interlok-service-tester-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3
- com.jayway.jsonpath:json-path:2.6.0

### interlok-service-tester-wiremock ###

#### New Dependencies ####
- com.github.tomakehurst:wiremock-jre8:2.28.0

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.3
- com.fasterxml.jackson.core:jackson-core:2.12.3
- com.fasterxml.jackson.core:jackson-databind:2.12.3

#### Removed Dependencies ####
- com.github.tomakehurst:wiremock:2.25.0

### interlok-sshtunnel ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.1.63

### interlok-stubs ###

#### Updated Dependencies ####
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

### interlok-swift ###

#### Updated Dependencies ####
- com.prowidesoftware:pw-swift-core:SRU2020-9.1.5

### interlok-vcs-git ###

#### Updated Dependencies ####
- com.github.mwiede:jsch:0.1.63
- org.eclipse.jgit:org.eclipse.jgit.ssh.jsch:5.11.1.202105131744-r
- org.eclipse.jgit:org.eclipse.jgit:5.11.1.202105131744-r

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- org.apache.cxf:cxf-rt-frontend-jaxws:3.4.3
- org.apache.cxf:cxf-rt-transports-http:3.4.3
- org.glassfish:javax.json:1.1.4

### interlok-xa-atomikos ###

#### Updated Dependencies ####
- org.awaitility:awaitility:4.1.0
