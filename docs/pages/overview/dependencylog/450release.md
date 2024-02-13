## Version 4.5.0-RELEASE ##

### interlok-activemq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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

#### Unchanged Dependencies ####
- org.apache.activemq.protobuf:activemq-protobuf:1.1
- org.apache.qpid:proton-j:0.33.10

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-amqp ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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

#### Unchanged Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:2.4.0
- org.apache.qpid:proton-j:0.33.10
- org.apache.qpid:proton-jms:0.12.2
- org.apache.qpid:qpid-amqp-1-0-client-jms:0.32
- org.apache.qpid:qpid-client:6.4.0

### interlok-apache-geode ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3
- org.jgroups:jgroups:4.2.4.Final
- org.springframework:spring-web:5.3.20

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.apache.geode:geode-core:1.14.4
- org.apache.shiro:shiro-core:1.9.0
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- commons-beanutils:commons-beanutils:1.9.4
- commons-codec:commons-codec:1.15

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-apache-http ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.13

### interlok-apache-http-async ###

#### Initial Dependencies ####
- com.adaptris:interlok-apache-http:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.apache.httpcomponents:httpasyncclient:4.1.5
- org.apache.httpcomponents:httpclient:4.5.13
- org.slf4j:slf4j-api:1.7.36

### interlok-apache-http5 ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.apache.httpcomponents.client5:httpclient5:5.1.3
- org.slf4j:slf4j-api:1.7.36

### interlok-artemis ###

#### New Dependencies ####
- org.jgroups:jgroups:4.2.4.Final

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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

#### Unchanged Dependencies ####
- org.apache.commons:commons-configuration2:2.7

### interlok-as400 ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- net.sf.jt400:jt400:9.1
- net.sf:cb2xml:0.92

### interlok-aws-common ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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
- com.adaptris:interlok-aws-common:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- org.apache.avro:avro:1.11.0
- org.apache.commons:commons-compress:1.21

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
- com.adaptris:interlok-aws-common:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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
- com.adaptris:interlok-aws-common:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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
- com.adaptris:interlok-aws-common:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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
- com.adaptris:interlok-aws-common:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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
- com.adaptris:interlok-aws-common:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.amazonaws:aws-java-sdk-core:1.12.228
- com.amazonaws:aws-java-sdk-sqs:1.12.228
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.0.8
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13

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
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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

#### Unchanged Dependencies ####
- com.microsoft.graph:microsoft-graph:2.5.0
- commons-codec:commons-codec:1.15
- org.codehaus.staxmate:stax2:2.1

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
- com.adaptris:interlok-apache-http:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.microsoft.azure:azure-documentdb:2.6.4
- commons-codec:commons-codec:1.15

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-azure-datalake ###

#### Updated Dependencies ####
- com.adaptris:interlok-azure-core:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-azure-mail ###

#### Updated Dependencies ####
- com.adaptris:interlok-azure-core:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-azure-onedrive ###

#### Updated Dependencies ####
- com.adaptris:interlok-azure-core:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-boot ###

### interlok-cassandra ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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
- com.adaptris:interlok-common:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-client-jmx ###

#### Updated Dependencies ####
- com.adaptris:interlok-client:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-cluster-manager ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE

#### Unchanged Dependencies ####
- org.jgroups:jgroups:4.2.4.Final

### interlok-common ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- org.apache.logging.log4j:log4j-1.2-api:2.17.2
- org.apache.logging.log4j:log4j-api:2.17.2
- org.apache.logging.log4j:log4j-core:2.17.2
- org.apache.logging.log4j:log4j-slf4j-impl:2.17.2
- org.eclipse.jetty.aggregate:jetty-all:9.4.46.v20220331
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:jul-to-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.19
- commons-io:commons-io:2.11.0
- commons-net:commons-net:3.8.0
- commons-pool:commons-pool:1.6
- javax.servlet:javax.servlet-api:4.0.1
- org.apache.commons:commons-lang3:3.12.0
- org.apache.commons:commons-pool2:2.11.1

### interlok-core ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.github.mwiede:jsch:0.2.1
- net.sf.saxon:Saxon-HE:11.3
- org.apache.activemq:activemq-client:5.17.1
- org.eclipse.jetty.aggregate:jetty-all:9.4.46.v20220331
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.mchange:c3p0:0.9.5.5
- com.sun.activation:jakarta.activation:1.2.2
- com.sun.mail:jakarta.mail:1.6.7
- com.thoughtworks.xstream:xstream:1.4.19
- com.zaxxer:HikariCP:5.0.1
- commons-io:commons-io:2.11.0
- commons-net:commons-net:3.8.0
- io.github.classgraph:classgraph:4.8.116
- jakarta.jms:jakarta.jms-api:2.0.3
- jakarta.validation:jakarta.validation-api:2.0.2
- javax.servlet:javax.servlet-api:4.0.1
- net.jodah:expiringmap:0.5.10
- net.sf.joost:joost:0.9.1
- org.apache-extras.beanshell:bsh:2.0b6
- org.apache.commons:commons-collections4:4.4
- org.apache.commons:commons-exec:1.3
- org.apache.commons:commons-lang3:3.12.0
- org.apache.commons:commons-pool2:2.11.1
- org.apache.commons:commons-text:1.9
- org.apache.derby:derby:10.15.2.0
- org.apache.derby:derbytools:10.15.2.0
- org.bouncycastle:bcmail-jdk15on:1.70
- org.bouncycastle:bcpkix-jdk15on:1.70
- org.bouncycastle:bcprov-jdk15on:1.70
- org.codehaus.jettison:jettison:1.2
- org.glassfish.external:opendmk_jdmkrt_jar:1.0-b01-ea
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.glassfish:javax.el:3.0.1-b12
- org.hibernate.javax.persistence:hibernate-jpa-2.1-api:1.0.2.Final
- org.hibernate.validator:hibernate-validator:6.1.7.Final
- org.quartz-scheduler:quartz:2.3.2
- xerces:xercesImpl:2.12.2

### interlok-core-apt ###

#### Unchanged Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.19
- jakarta.validation:jakarta.validation-api:2.0.2

### interlok-csv ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-stax:4.5.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- net.sf.supercsv:super-csv:2.4.0

### interlok-csv-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-csv:4.5.0-RELEASE
- com.adaptris:interlok-json:4.5.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-csv-schema ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.gilt:gfc-semver_2.11:0.0.5
- org.scala-lang.plugins:scala-continuations-library_2.11:1.0.3
- org.scala-lang:scala-library:2.11.12
- uk.gov.nationalarchives:csv-validator-java-api:1.1.5

### interlok-edi-legacy ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-edi-stream ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- javax.cache:cache-api:1.1.1

### interlok-ehcache ###

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- net.sf.ehcache:ehcache:2.10.9.2

### interlok-elastic-common ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:
- com.fasterxml.jackson:jackson-bom:2.13.3
- org.elasticsearch:elasticsearch:7.15.1

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-csv:4.5.0-RELEASE
- com.adaptris:interlok-json:4.5.0-RELEASE
- joda-time:joda-time:2.10.14
- org.apache.logging.log4j:log4j-api:2.17.2
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.7.0
- commons-collections:commons-collections:3.2.2
- net.sf.supercsv:super-csv:2.4.0
- org.apache.commons:commons-csv:1.9.0
- org.yaml:snakeyaml:1.30

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.15.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.15.1

### interlok-elastic-rest ###

#### New Dependencies ####
- com.adaptris:interlok-apache-http-async:4.5.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:
- com.fasterxml.jackson.dataformat:jackson-dataformat-smile:
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-elastic-common:4.5.0-RELEASE
- joda-time:joda-time:2.10.14
- org.apache.logging.log4j:log4j-api:2.17.2
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.7.0
- commons-codec:commons-codec:1.15
- commons-collections:commons-collections:3.2.2
- org.apache.httpcomponents:httpclient:4.5.13
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.15.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.15.1
- org.yaml:snakeyaml:1.30

#### Removed Dependencies ####
- com.adaptris:interlok-csv:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-excel ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.apache.commons:commons-compress:1.21
- org.apache.poi:poi-ooxml:4.1.2
- org.apache.poi:poi:4.1.2

### interlok-exec ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.apache.commons:commons-exec:1.3

### interlok-expressions ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.apache-extras.beanshell:bsh:2.0b6

### interlok-failover ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.jgroups:jgroups:4.2.4.Final

### interlok-filesystem ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.hierynomus:smbj:0.11.5
- org.apache.tika:tika-core:2.4.0
- org.json:json:20220320
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.apache.commons:commons-compress:1.21

### interlok-flatfile ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE

### interlok-flyway ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.flywaydb:flyway-core:8.5.11

#### Unchanged Dependencies ####
- commons-collections:commons-collections:3.2.2

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-oauth-gcloud:4.5.0-RELEASE
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

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-hpcc ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.apache.commons:commons-exec:1.3
- oro:oro:2.0.8

### interlok-installer ###

#### Unchanged Dependencies ####
- org.gradle:gradle-tooling-api:7.2
- org.openjfx:javafx-base:11.0.2
- org.openjfx:javafx-controls:11.0.2
- org.openjfx:javafx-fxml:11.0.2
- org.openjfx:javafx-graphics:11.0.2

### interlok-jclouds-aws-sts ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-jclouds-common:4.5.0-RELEASE
- org.apache.jclouds.api:sts:2.5.0
- org.slf4j:slf4j-api:1.7.36

### interlok-jclouds-blobstore ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-jclouds-common:4.5.0-RELEASE
- org.apache.jclouds:jclouds-blobstore:2.5.0
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- javax.xml.bind:jaxb-api:2.3.1

### interlok-jclouds-common ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.google.guava:guava:31.1-jre
- org.apache.jclouds:jclouds-core:2.5.0
- org.slf4j:slf4j-api:1.7.36

### interlok-jdbc ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.google.guava:guava:31.1-jre
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- org.codehaus.staxmate:stax2:2.1

### interlok-jms-oracleaq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.oracle:ojdbc14:10.2.0.1.0
- com.oracle:oracle-aq:1.0

### interlok-jms-sonicmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.aurea:sonic-channel:8.5.0
- com.aurea:sonic-client:8.5.0
- com.aurea:sonic-crypto:8.5.0
- com.aurea:sonic-xa:8.5.0
- com.aurea:sonic-xmessage:8.5.0

### interlok-jmx-activemq ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.5.0-RELEASE
- org.apache.activemq:activemq-client:5.17.1
- org.slf4j:slf4j-api:1.7.36
- org.springframework:spring-aop:5.3.20
- org.springframework:spring-beans:5.3.20
- org.springframework:spring-context:5.3.20
- org.springframework:spring-core:5.3.20
- org.springframework:spring-jms:5.3.20

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.19
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-jmx-amqp ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.5.0-RELEASE
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

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.19
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.qpid:proton-j:0.33.10
- org.apache.qpid:proton-jms:0.12.2
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-jmx-jms-common ###

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.36
- org.springframework:spring-aop:5.3.20
- org.springframework:spring-beans:5.3.20
- org.springframework:spring-context:5.3.20
- org.springframework:spring-core:5.3.20
- org.springframework:spring-jms:5.3.20

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.19
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-jmx-jms-stubs ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.5.0-RELEASE
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

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.19
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- javax.management.j2ee:javax.management.j2ee-api:1.1.2
- junit:junit:4.13.2
- org.apache.activemq.protobuf:activemq-protobuf:1.1
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-jmx-solace ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.5.0-RELEASE
- com.solacesystems:sol-common:10.14.0
- com.solacesystems:sol-jcsmp:10.14.0
- com.solacesystems:sol-jms:10.14.0
- org.slf4j:slf4j-api:1.7.36
- org.springframework:spring-aop:5.3.20
- org.springframework:spring-beans:5.3.20
- org.springframework:spring-context:5.3.20
- org.springframework:spring-core:5.3.20
- org.springframework:spring-jms:5.3.20

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- com.thoughtworks.xstream:xstream:1.4.19
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-jmx-sonicmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.5.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.aurea:sonic-channel:8.5.0
- com.aurea:sonic-client:8.5.0
- com.aurea:sonic-crypto:8.5.0
- com.aurea:sonic-xa:8.5.0
- com.aurea:sonic-xmessage:8.5.0

### interlok-jolokia ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.eclipse.jetty.aggregate:jetty-all:9.4.46.v20220331

#### Unchanged Dependencies ####
- org.jolokia:jolokia-core:1.7.1
- org.jolokia:jolokia-jsr160:1.7.1

### interlok-jq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- net.thisptr:jackson-jq-extra:1.0.0-preview.20210928
- net.thisptr:jackson-jq:1.0.0-preview.20210928

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-jruby ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.jruby:jruby:9.3.4.0
- org.slf4j:slf4j-api:1.7.36

### interlok-jslt ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
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
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.bazaarvoice.jolt:jolt-core:0.1.7
- com.bazaarvoice.jolt:json-utils:0.1.7
- com.flipkart.zjsonpatch:zjsonpatch:0.4.12
- com.google.guava:guava:31.1-jre
- org.json:json:20220320
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.7.0
- commons-beanutils:commons-beanutils:1.9.4
- commons-collections:commons-collections:3.2.2
- net.sf.json-lib:json-lib:2.4
- xerces:xercesImpl:2.12.2
- xom:xom:1.3.7

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
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-json:4.5.0-RELEASE
- com.adaptris:interlok-stax:4.5.0-RELEASE
- com.google.code.gson:gson:2.9.0
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.github.jsurfer:jsurfer-core:1.6.3
- com.github.jsurfer:jsurfer-gson:1.6.3
- com.github.jsurfer:jsurfer-jackson:1.6.3
- com.github.jsurfer:jsurfer-jsonsimple:1.6.3
- de.odysseus.staxon:staxon:1.3

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-json-web-token ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- io.jsonwebtoken:jjwt-api:0.11.5
- io.jsonwebtoken:jjwt-impl:0.11.5
- io.jsonwebtoken:jjwt-jackson:0.11.5
- org.json:json:20220320
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.70
- org.bouncycastle:bcprov-jdk15on:1.70

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.5

### interlok-jsr107-cache ###

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- javax.cache:cache-api:1.1.1

### interlok-kafka ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3
- org.apache.zookeeper:zookeeper:3.8.0

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- io.netty:netty-codec:4.1.77.Final
- io.netty:netty-handler:4.1.77.Final
- io.netty:netty-transport-native-epoll:4.1.77.Final
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- commons-collections:commons-collections:3.2.2
- org.apache.kafka:kafka-clients:2.4.1
- org.apache.kafka:kafka_2.11:2.4.1

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-kie ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.drools:drools-compiler:7.70.0.Final
- org.drools:drools-core:7.70.0.Final
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.19
- commons-codec:commons-codec:1.15
- org.apache.commons:commons-collections4:4.4

### interlok-licensing ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-licensing-demo ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-logging ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-api:2.17.2
- org.apache.logging.log4j:log4j-core:2.17.2

### interlok-mail ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE

#### Unchanged Dependencies ####
- com.sun.mail:jakarta.mail:1.6.7

### interlok-mongodb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-json:4.5.0-RELEASE
- org.mongodb:mongodb-driver:3.12.11
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-mqtt ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- javax.transaction:jta:1.1
- org.apache.httpcomponents:httpclient:4.5.13
- org.eclipse.paho:org.eclipse.paho.client.mqttv3:1.2.5

### interlok-msmq-javonet ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.javonet:javonet:1.4-hf15

### interlok-nats ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- io.nats:jnats:2.15.1

### interlok-oauth-azure ###

#### New Dependencies ####
- com.google.code.gson:gson:2.9.0

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.nimbusds:nimbus-jose-jwt:9.22
- net.minidev:json-smart:2.4.8
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.microsoft.azure:adal4j:1.6.7

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.fasterxml.jackson.core:jackson-core:2.13.3
- com.google.auth:google-auth-library-oauth2-http:1.7.0
- com.google.guava:guava:31.1-jre
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13

### interlok-oauth-generic ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:4.5.0-RELEASE
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.7.0

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-oauth-salesforce ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-okhttp ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.squareup.okhttp3:okhttp:4.9.3

### interlok-pdf ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.google.guava:guava:31.1-jre
- org.apache.pdfbox:fontbox:2.0.26
- org.apache.pdfbox:pdfbox-tools:2.0.26
- org.apache.pdfbox:pdfbox:2.0.26
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- commons-io:commons-io:2.11.0
- net.sf.cssbox:pdf2dom:2.0.1
- org.apache.xmlgraphics:fop:2.7
- xerces:xercesImpl:2.12.2

### interlok-pgp ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.bouncycastle:bcpg-jdk15on:1.70
- org.bouncycastle:bcprov-jdk15on:1.70

### interlok-profiler ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.aspectj:aspectjrt:1.9.9.1
- org.aspectj:aspectjtools:1.9.9.1
- org.aspectj:aspectjweaver:1.9.9.1
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.apache.commons:commons-math3:3.6.1

### interlok-proxy ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.5.0-RELEASE
- com.adaptris:interlok-client:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.apache.httpcomponents.client5:httpclient5:5.1.3

### interlok-rabbitmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.rabbitmq:amqp-client:5.14.2
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-rest-base ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.5.0-RELEASE
- com.adaptris:interlok-client:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE

### interlok-rest-cluster ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.5.0-RELEASE
- com.adaptris:interlok-client:4.5.0-RELEASE
- com.adaptris:interlok-cluster-manager:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-rest-base:4.5.0-RELEASE

### interlok-rest-health-check ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.5.0-RELEASE
- com.adaptris:interlok-client:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-rest-base:4.5.0-RELEASE

### interlok-rest-metrics-jvm ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.5.0-RELEASE
- com.adaptris:interlok-client:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-rest-base:4.5.0-RELEASE
- io.micrometer:micrometer-core:1.9.0

#### Unchanged Dependencies ####
- io.github.mweirauch:micrometer-jvm-extras:0.2.2

### interlok-rest-metrics-profiler ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.5.0-RELEASE
- com.adaptris:interlok-client:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-profiler:4.5.0-RELEASE
- com.adaptris:interlok-rest-base:4.5.0-RELEASE
- com.adaptris:interlok-rest-metrics-jvm:4.5.0-RELEASE

### interlok-rest-provider-datadog ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.5.0-RELEASE
- com.adaptris:interlok-client:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-rest-base:4.5.0-RELEASE
- com.adaptris:interlok-rest-metrics-jvm:4.5.0-RELEASE
- io.micrometer:micrometer-registry-datadog:1.9.0

### interlok-rest-provider-prometheus ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.5.0-RELEASE
- com.adaptris:interlok-client:4.5.0-RELEASE
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-rest-base:4.5.0-RELEASE
- com.adaptris:interlok-rest-metrics-jvm:4.5.0-RELEASE
- io.micrometer:micrometer-registry-prometheus:1.9.0

### interlok-sap ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.sap:sapidoc3:3.0.12
- com.sap:sapjco3:3.0.13
- org.apache.ant:ant:1.10.12

### interlok-service-tester ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-varsub:4.5.0-RELEASE
- com.adaptris:interlok-xinclude:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- commons-io:commons-io:2.11.0

### interlok-service-tester-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:
- com.fasterxml.jackson.core:jackson-databind:
- com.fasterxml.jackson:jackson-bom:2.13.3

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-service-tester:4.5.0-RELEASE
- org.json:json:20220320
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.jayway.jsonpath:json-path:2.7.0
- org.skyscreamer:jsonassert:1.5.0

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
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-service-tester:4.5.0-RELEASE
- com.github.tomakehurst:wiremock-jre8:2.33.2
- com.google.guava:guava:31.1-jre
- org.slf4j:slf4j-api:1.7.36

#### Removed Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1

### interlok-service-tester-xml ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-service-tester:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- xmlunit:xmlunit:1.6

### interlok-solace ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.solacesystems:sol-common:10.14.0
- com.solacesystems:sol-jcsmp:10.14.0
- com.solacesystems:sol-jms:10.14.0
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- net.jodah:expiringmap:0.5.10

### interlok-sshtunnel ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.github.mwiede:jsch:0.2.1
- org.slf4j:slf4j-api:1.7.36

### interlok-stax ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-stubs ###

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- junit:junit:4.13.2

### interlok-swift ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.prowidesoftware:pw-swift-core:SRU2021-9.2.13
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

### interlok-tibco ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.tibco:tibjms:6.3.0
- com.tibco:tibrv:7.5.1

### interlok-triggered ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-varsub ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE

### interlok-vcs-git ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.github.mwiede:jsch:0.2.1
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- commons-lang:commons-lang:2.6
- org.apache.httpcomponents:httpclient:4.5.13
- org.eclipse.jgit:org.eclipse.jgit.ssh.jsch:5.13.0.202109080827-r
- org.eclipse.jgit:org.eclipse.jgit:5.13.0.202109080827-r

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.apache.cxf:cxf-rt-frontend-jaxws:3.5.2
- org.apache.cxf:cxf-rt-transports-http:3.5.2
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.sun.xml.messaging.saaj:saaj-impl:1.5.1
- jakarta.xml.bind:jakarta.xml.bind-api:2.3.2
- javax.jws:jsr181-api:1.0-MR1
- javax.xml.soap:saaj-api:1.3.5
- javax.xml.ws:jaxws-api:2.3.1
- org.eclipse:yasson:1.0.1
- org.glassfish.jaxb:jaxb-runtime:2.3.2
- org.glassfish:javax.json:1.1.4

### interlok-webspheremq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.ibm.mq:com.ibm.mq.allclient:9.2.5.0
- org.slf4j:jcl-over-slf4j:1.7.36
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- org.apache.geronimo.specs:geronimo-j2ee-connector_1.6_spec:1.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1

### interlok-work-unit ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-activemq ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- com.adaptris:interlok-xa-jms:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-atomikos ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- com.adaptris:interlok-xa-jms:4.5.0-RELEASE
- org.awaitility:awaitility:4.2.0
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.atomikos:transactions-jms:3.8.0

### interlok-xa-jms ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-solace ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- com.adaptris:interlok-solace:4.5.0-RELEASE
- com.adaptris:interlok-xa-jms:4.5.0-RELEASE
- com.solacesystems:sol-common:10.14.0
- com.solacesystems:sol-jcsmp:10.14.0
- com.solacesystems:sol-jms:10.14.0
- org.slf4j:slf4j-api:1.7.36

### interlok-xa-tibco ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- com.adaptris:interlok-tibco:4.5.0-RELEASE
- com.adaptris:interlok-xa-jms:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- com.tibco:tibjms:6.3.0
- com.tibco:tibrv:7.5.1

### interlok-xa-wmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- com.adaptris:interlok-webspheremq:4.5.0-RELEASE
- com.adaptris:interlok-xa-jms:4.5.0-RELEASE
- com.ibm.mq:com.ibm.mq.allclient:9.2.5.0
- org.slf4j:slf4j-api:1.7.36

### interlok-xinclude ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE

### interlok-xml-security ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.5.0-RELEASE
- com.adaptris:interlok-core:4.5.0-RELEASE
- com.adaptris:interlok-licensing:4.5.0-RELEASE
- org.slf4j:slf4j-api:1.7.36

#### Unchanged Dependencies ####
- iaik:iaik-cms:4.0
- iaik:iaik-jce:3.16
- iaik:iaik-xsect:1.11
