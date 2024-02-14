## Version 3.12.0-RELEASE ##

### interlok-activemq ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.google.guava:guava:30.1-jre
- org.apache.qpid:proton-j:0.33.8
- org.springframework:spring-beans:4.3.30.RELEASE
- org.springframework:spring-context:4.3.30.RELEASE

### interlok-amqp ###

#### Updated Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:2.2.0
- io.netty:netty-buffer:4.1.56.Final
- io.netty:netty-codec-http:4.1.56.Final
- io.netty:netty-codec:4.1.56.Final
- io.netty:netty-common:4.1.56.Final
- io.netty:netty-handler:4.1.56.Final
- io.netty:netty-transport-native-epoll:4.1.56.Final
- io.netty:netty-transport-native-kqueue:4.1.56.Final
- io.netty:netty-transport-native-unix-common:4.1.56.Final
- io.netty:netty-transport:4.1.56.Final
- org.apache.qpid:proton-j:0.33.8
- org.apache.qpid:qpid-jms-client:0.56.0

### interlok-apache-geode ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.1
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- org.apache.httpcomponents:httpclient:4.5.13

#### Updated Dependencies ####
- org.apache.geode:geode-core:1.13.1
- org.apache.shiro:shiro-core:1.7.0

### interlok-artemis ###

#### Updated Dependencies ####
- io.netty:netty-buffer:4.1.56.Final
- io.netty:netty-codec-http:4.1.56.Final
- io.netty:netty-codec:4.1.56.Final
- io.netty:netty-common:4.1.56.Final
- io.netty:netty-handler:4.1.56.Final
- io.netty:netty-transport-native-epoll:4.1.56.Final
- io.netty:netty-transport-native-kqueue:4.1.56.Final
- io.netty:netty-transport-native-unix-common:4.1.56.Final
- io.netty:netty-transport:4.1.56.Final
- org.apache.activemq:artemis-jms-server:2.16.0
- org.apache.activemq:artemis-server:2.16.0

### interlok-aws-common ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-sts:1.11.930

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.930
- com.fasterxml.jackson.core:jackson-annotations:2.12.1
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.12.1

### interlok-aws-kinesis ###

#### Updated Dependencies ####
- com.amazonaws:amazon-kinesis-producer:0.14.2
- com.amazonaws:aws-java-sdk-kinesis:1.11.930
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.google.protobuf:protobuf-java:3.14.0

### interlok-aws-kms ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-kms:1.11.930

### interlok-aws-s3 ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.930

### interlok-aws-sns ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.930

#### Removed Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.892

### interlok-aws-sqs ###

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sqs:1.11.930
- com.fasterxml.jackson.core:jackson-databind:2.12.1

#### Removed Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.892

### interlok-azure-core ###

#### New Dependencies ####
- com.fasterxml.jackson.dataformat:jackson-dataformat-xml:2.12.1
- com.fasterxml.jackson.datatype:jackson-datatype-jsr310:2.12.1
- io.netty:netty-codec-http2:4.1.56.Final
- io.netty:netty-codec-http:4.1.56.Final
- io.netty:netty-codec:4.1.56.Final
- io.netty:netty-handler-proxy:4.1.56.Final
- io.netty:netty-handler:4.1.56.Final
- io.netty:netty-transport-native-epoll:4.1.56.Final
- io.netty:netty-transport-native-kqueue:4.1.56.Final
- io.netty:netty-transport-native-unix-common:4.1.56.Final

#### Updated Dependencies ####
- com.azure:azure-identity:1.2.1
- com.azure:azure-storage-file-datalake:12.3.0
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.google.guava:guava:30.1-jre
- com.microsoft.azure:msal4j:1.8.1
- com.microsoft.graph:microsoft-graph:2.5.0

### interlok-azure-cosmosdb ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.microsoft.azure:azure-documentdb:2.6.1

### interlok-cassandra ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.google.guava:guava:30.1-jre
- io.netty:netty-codec:4.1.56.Final
- io.netty:netty-handler:4.1.56.Final
- io.netty:netty-transport-native-epoll:4.1.56.Final

### interlok-client ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-1.2-api:2.14.0
- org.apache.logging.log4j:log4j-api:2.14.0
- org.apache.logging.log4j:log4j-core:2.14.0
- org.mockito:mockito-core:3.7.0
- org.mockito:mockito-inline:3.7.0

### interlok-client-jmx ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-1.2-api:2.14.0
- org.apache.logging.log4j:log4j-api:2.14.0
- org.apache.logging.log4j:log4j-core:2.14.0
- org.mockito:mockito-core:3.7.0
- org.mockito:mockito-inline:3.7.0

### interlok-common ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.15
- org.apache.logging.log4j:log4j-1.2-api:2.14.0
- org.apache.logging.log4j:log4j-api:2.14.0
- org.apache.logging.log4j:log4j-core:2.14.0
- org.apache.logging.log4j:log4j-slf4j-impl:2.14.0
- org.eclipse.jetty.aggregate:jetty-all:9.4.36.v20210114
- org.mockito:mockito-core:3.7.0
- org.mockito:mockito-inline:3.7.0

### interlok-core ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.15
- net.sf.saxon:Saxon-HE:10.3
- org.apache.activemq:artemis-jms-server:2.16.0
- org.bouncycastle:bcmail-jdk15on:1.68
- org.bouncycastle:bcpkix-jdk15on:1.68
- org.bouncycastle:bcprov-jdk15on:1.68
- org.eclipse.jetty.aggregate:jetty-all:9.4.36.v20210114
- org.jruby:jruby-complete:9.2.14.0
- org.mockito:mockito-core:3.7.0
- org.mockito:mockito-inline:3.7.0
- xerces:xercesImpl:2.12.1

### interlok-core-apt ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.15

### interlok-csv-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1

### interlok-elastic-common ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- joda-time:joda-time:2.10.9

### interlok-elastic-rest ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- joda-time:joda-time:2.10.9

### interlok-filesystem ###

#### Updated Dependencies ####
- org.apache.tika:tika-core:1.25
- org.json:json:20201115

### interlok-flyway ###

#### Updated Dependencies ####
- org.flywaydb:flyway-core:7.3.2

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- io.netty:netty-codec-http2:4.1.56.Final
- io.netty:netty-codec-http:4.1.56.Final

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.google.cloud:google-cloud-pubsub:1.110.1
- com.google.guava:guava:30.1-jre
- com.google.protobuf:protobuf-java-util:3.14.0
- com.google.protobuf:protobuf-java:3.14.0
- io.grpc:grpc-alts:1.34.1
- io.grpc:grpc-auth:1.34.1
- io.grpc:grpc-netty:1.34.1
- io.grpc:grpc-protobuf:1.34.1
- io.grpc:grpc-stub:1.34.1
- io.netty:netty-codec:4.1.56.Final
- io.netty:netty-handler:4.1.56.Final
- io.netty:netty-transport-native-epoll:4.1.56.Final

### interlok-http-multipart ###

#### Initial Dependencies ####
- com.sun.mail:jakarta.mail:1.6.7

### interlok-jclouds-common ###

#### Updated Dependencies ####
- com.google.guava:guava:30.1-jre

### interlok-jmx-activemq ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.15
- org.springframework:spring-aop:4.3.30.RELEASE
- org.springframework:spring-beans:4.3.30.RELEASE
- org.springframework:spring-context:4.3.30.RELEASE
- org.springframework:spring-core:4.3.30.RELEASE
- org.springframework:spring-jms:4.3.30.RELEASE

### interlok-jmx-amqp ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.15
- io.netty:netty-buffer:4.1.56.Final
- io.netty:netty-codec-http:4.1.56.Final
- io.netty:netty-codec:4.1.56.Final
- io.netty:netty-common:4.1.56.Final
- io.netty:netty-handler:4.1.56.Final
- io.netty:netty-transport-native-epoll:4.1.56.Final
- io.netty:netty-transport-native-kqueue:4.1.56.Final
- io.netty:netty-transport-native-unix-common:4.1.56.Final
- io.netty:netty-transport:4.1.56.Final
- org.apache.qpid:proton-j:0.33.8
- org.apache.qpid:qpid-jms-client:0.56.0
- org.springframework:spring-aop:4.3.30.RELEASE
- org.springframework:spring-beans:4.3.30.RELEASE
- org.springframework:spring-context:4.3.30.RELEASE
- org.springframework:spring-core:4.3.30.RELEASE
- org.springframework:spring-jms:4.3.30.RELEASE

### interlok-jmx-jms-common ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.15
- org.springframework:spring-aop:4.3.30.RELEASE
- org.springframework:spring-beans:4.3.30.RELEASE
- org.springframework:spring-context:4.3.30.RELEASE
- org.springframework:spring-core:4.3.30.RELEASE
- org.springframework:spring-jms:4.3.30.RELEASE

### interlok-jmx-jms-stubs ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.thoughtworks.xstream:xstream:1.4.15
- org.springframework:spring-aop:4.3.30.RELEASE
- org.springframework:spring-beans:4.3.30.RELEASE
- org.springframework:spring-context:4.3.30.RELEASE
- org.springframework:spring-core:4.3.30.RELEASE
- org.springframework:spring-jms:4.3.30.RELEASE

### interlok-jmx-solace ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.15
- org.springframework:spring-aop:4.3.30.RELEASE
- org.springframework:spring-beans:4.3.30.RELEASE
- org.springframework:spring-context:4.3.30.RELEASE
- org.springframework:spring-core:4.3.30.RELEASE
- org.springframework:spring-jms:4.3.30.RELEASE

### interlok-jq ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1

### interlok-jruby ###

#### Updated Dependencies ####
- org.jruby:jruby:9.2.14.0

### interlok-jslt ###

#### Initial Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.schibsted.spt.data:jslt:0.1.11

### interlok-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.12.1
- com.google.guava:guava:30.1-jre
- org.json:json:20201115
- xerces:xercesImpl:2.12.1

### interlok-json-web-token ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- org.bouncycastle:bcpg-jdk15on:1.68
- org.bouncycastle:bcprov-jdk15on:1.68
- org.json:json:20201115

### interlok-kafka ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- io.netty:netty-codec:4.1.56.Final
- io.netty:netty-handler:4.1.56.Final
- io.netty:netty-transport-native-epoll:4.1.56.Final

### interlok-kie ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.15
- org.drools:drools-compiler:7.47.0.Final
- org.drools:drools-core:7.47.0.Final

### interlok-logging ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-api:2.14.0
- org.apache.logging.log4j:log4j-core:2.14.0

### interlok-mongodb ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.google.auth:google-auth-library-oauth2-http:0.22.2
- com.google.guava:guava:30.1-jre

### interlok-oauth-generic ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1

### interlok-oauth-salesforce ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1

### interlok-pdf ###

#### Updated Dependencies ####
- com.google.guava:guava:30.1-jre
- org.apache.pdfbox:fontbox:2.0.22
- org.apache.pdfbox:pdfbox-tools:2.0.22
- org.apache.pdfbox:pdfbox:2.0.22
- xerces:xercesImpl:2.12.1

### interlok-pgp ###

#### Updated Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.68
- org.bouncycastle:bcprov-jdk15on:1.68

### interlok-service-tester-json ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- org.json:json:20201115

### interlok-service-tester-wiremock ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.12.1
- com.fasterxml.jackson.core:jackson-core:2.12.1
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.google.guava:guava:30.1-jre

### interlok-shell ###

#### Updated Dependencies ####
- org.bouncycastle:bcpkix-jdk15on:1.68
- org.bouncycastle:bcprov-jdk15on:1.68
- org.codehaus.groovy:groovy-all:2.5.14

### interlok-stubs ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.15
- net.sf.saxon:Saxon-HE:10.3
- org.apache.activemq:artemis-jms-server:2.16.0
- org.bouncycastle:bcmail-jdk15on:1.68
- org.bouncycastle:bcpkix-jdk15on:1.68
- org.bouncycastle:bcprov-jdk15on:1.68
- org.eclipse.jetty.aggregate:jetty-all:9.4.36.v20210114
- org.jruby:jruby-complete:9.2.14.0
- org.mockito:mockito-core:3.7.0
- org.mockito:mockito-inline:3.7.0
- xerces:xercesImpl:2.12.1

### interlok-swift ###

#### Updated Dependencies ####
- com.prowidesoftware:pw-swift-core:SRU2020-9.1.3

### interlok-vcs-git ###

#### Updated Dependencies ####
- org.eclipse.jgit:org.eclipse.jgit.ssh.jsch:5.10.0.202012080955-r
- org.eclipse.jgit:org.eclipse.jgit:5.10.0.202012080955-r

### interlok-vertx ###

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.1
- com.hazelcast:hazelcast:4.1.1
- io.vertx:vertx-core:4.0.0
- io.vertx:vertx-hazelcast:4.0.0

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- org.apache.cxf:cxf-rt-frontend-jaxws:3.4.2
- org.apache.cxf:cxf-rt-transports-http:3.4.2
