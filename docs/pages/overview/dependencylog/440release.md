## Version 4.4.0-RELEASE ##

### interlok-activemq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- org.springframework:spring-beans:5.3.15
- org.springframework:spring-context:5.3.15

#### Unchanged Dependencies ####
- com.google.guava:guava:31.0.1-jre
- org.apache.activemq.protobuf:activemq-protobuf:1.1
- org.apache.activemq:activemq-amqp:5.16.3
- org.apache.activemq:activemq-broker:5.16.3
- org.apache.activemq:activemq-client:5.16.3
- org.apache.activemq:activemq-jaas:5.16.3
- org.apache.activemq:activemq-kahadb-store:5.16.3
- org.apache.activemq:activemq-mqtt:5.16.3
- org.apache.activemq:activemq-spring:5.16.3
- org.apache.activemq:activemq-stomp:5.16.3
- org.apache.qpid:proton-j:0.33.10

### interlok-amqp ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.rabbitmq.jms:rabbitmq-jms:2.4.0
- com.rabbitmq:amqp-client:5.14.1
- io.netty:netty-buffer:4.1.73.Final
- io.netty:netty-codec-http:4.1.73.Final
- io.netty:netty-codec:4.1.73.Final
- io.netty:netty-common:4.1.73.Final
- io.netty:netty-handler:4.1.73.Final
- io.netty:netty-transport-native-epoll:4.1.73.Final
- io.netty:netty-transport-native-kqueue:4.1.73.Final
- io.netty:netty-transport-native-unix-common:4.1.73.Final
- io.netty:netty-transport:4.1.73.Final
- org.apache.qpid:qpid-jms-client:1.5.0
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.apache.qpid:proton-j:0.33.10
- org.apache.qpid:proton-jms:0.12.2
- org.apache.qpid:qpid-amqp-1-0-client-jms:0.32
- org.apache.qpid:qpid-client:6.4.0

### interlok-apache-geode ###

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- org.apache.geode:geode-core:1.14.3
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- commons-beanutils:commons-beanutils:1.9.4
- commons-codec:commons-codec:1.15
- org.apache.shiro:shiro-core:1.8.0

### interlok-apache-http ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.13

### interlok-apache-http5 ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.apache.httpcomponents.client5:httpclient5:5.1.2
- org.slf4j:slf4j-api:1.7.35

### interlok-artemis ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- io.netty:netty-buffer:4.1.73.Final
- io.netty:netty-codec-http:4.1.73.Final
- io.netty:netty-codec:4.1.73.Final
- io.netty:netty-common:4.1.73.Final
- io.netty:netty-handler:4.1.73.Final
- io.netty:netty-transport-native-epoll:4.1.73.Final
- io.netty:netty-transport-native-kqueue:4.1.73.Final
- io.netty:netty-transport-native-unix-common:4.1.73.Final
- io.netty:netty-transport:4.1.73.Final
- org.apache.activemq:artemis-jms-server:2.20.0
- org.apache.activemq:artemis-server:2.20.0

#### Unchanged Dependencies ####
- org.apache.commons:commons-configuration2:2.7

### interlok-as400 ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- net.sf.jt400:jt400:9.1
- net.sf:cb2xml:0.92

### interlok-aws-common ###

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.amazonaws:aws-java-sdk-core:1.12.150
- com.amazonaws:aws-java-sdk-sts:1.12.150
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

### interlok-aws-kinesis ###

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.amazonaws:amazon-kinesis-client:1.14.7
- com.amazonaws:aws-java-sdk-core:1.12.150
- com.amazonaws:aws-java-sdk-kinesis:1.12.150
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1
- com.google.protobuf:protobuf-java:3.19.4
- io.netty:netty-buffer:4.1.73.Final
- io.netty:netty-codec-http:4.1.73.Final
- io.netty:netty-codec:4.1.73.Final
- io.netty:netty-common:4.1.73.Final
- io.netty:netty-handler:4.1.73.Final
- io.netty:netty-transport-native-epoll:4.1.73.Final
- io.netty:netty-transport-native-kqueue:4.1.73.Final
- io.netty:netty-transport-native-unix-common:4.1.73.Final
- io.netty:netty-transport:4.1.73.Final
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.amazonaws:amazon-kinesis-producer:0.14.10
- com.google.guava:guava:31.0.1-jre
- commons-codec:commons-codec:1.15
- org.apache.avro:avro:1.11.0
- org.apache.commons:commons-compress:1.21

### interlok-aws-kinesis-sdk ###

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.amazonaws:aws-java-sdk-core:1.12.150
- com.amazonaws:aws-java-sdk-kinesis:1.12.150
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

### interlok-aws-kms ###

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.amazonaws:aws-java-sdk-core:1.12.150
- com.amazonaws:aws-java-sdk-kms:1.12.150
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

### interlok-aws-s3 ###

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.amazonaws:aws-java-sdk-core:1.12.150
- com.amazonaws:aws-java-sdk-s3:1.12.150
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

### interlok-aws-sns ###

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.amazonaws:aws-java-sdk-core:1.12.150
- com.amazonaws:aws-java-sdk-sns:1.12.150
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

### interlok-aws-sqs ###

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.amazonaws:aws-java-sdk-core:1.12.150
- com.amazonaws:aws-java-sdk-sqs:1.12.150
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.0.8
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13

### interlok-azure-core ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.azure:azure-identity:1.4.3
- com.azure:azure-storage-file-datalake:12.7.3
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-xml:2.13.1
- com.fasterxml.jackson.datatype:jackson-datatype-jsr310:2.13.1
- io.netty:netty-codec-http2:4.1.73.Final
- io.netty:netty-codec-http:4.1.73.Final
- io.netty:netty-codec:4.1.73.Final
- io.netty:netty-handler-proxy:4.1.73.Final
- io.netty:netty-handler:4.1.73.Final
- io.netty:netty-transport-native-epoll:4.1.73.Final
- io.netty:netty-transport-native-kqueue:4.1.73.Final
- io.netty:netty-transport-native-unix-common:4.1.73.Final
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.google.guava:guava:31.0.1-jre
- com.microsoft.azure:msal4j:1.11.0
- com.microsoft.graph:microsoft-graph:2.5.0
- commons-codec:commons-codec:1.15
- net.minidev:json-smart:2.4.7
- org.codehaus.staxmate:stax2:2.1

### interlok-azure-cosmosdb ###

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.microsoft.azure:azure-documentdb:2.6.4
- commons-codec:commons-codec:1.15

### interlok-azure-datalake ###

#### Updated Dependencies ####
- com.adaptris:interlok-azure-core:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-azure-mail ###

#### Updated Dependencies ####
- com.adaptris:interlok-azure-core:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-azure-onedrive ###

#### Updated Dependencies ####
- com.adaptris:interlok-azure-core:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-boot ###

### interlok-cassandra ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- io.netty:netty-codec:4.1.73.Final
- io.netty:netty-handler:4.1.73.Final
- io.netty:netty-transport-native-epoll:4.1.73.Final
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.datastax.cassandra:cassandra-driver-core:3.11.0
- com.datastax.cassandra:cassandra-driver-mapping:3.11.0
- com.google.guava:guava:31.0.1-jre

### interlok-client ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-client-jmx ###

#### Updated Dependencies ####
- com.adaptris:interlok-client:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-cluster-manager ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE

#### Unchanged Dependencies ####
- org.jgroups:jgroups:4.2.4.Final

### interlok-common ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.thoughtworks.xstream:xstream:1.4.19
- org.apache.logging.log4j:log4j-1.2-api:2.17.1
- org.apache.logging.log4j:log4j-api:2.17.1
- org.apache.logging.log4j:log4j-core:2.17.1
- org.apache.logging.log4j:log4j-slf4j-impl:2.17.1
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:jul-to-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- commons-io:commons-io:2.11.0
- commons-net:commons-net:3.8.0
- commons-pool:commons-pool:1.6
- javax.servlet:javax.servlet-api:4.0.1
- org.apache.commons:commons-lang3:3.12.0
- org.apache.commons:commons-pool2:2.11.1
- org.eclipse.jetty.aggregate:jetty-all:9.4.44.v20210927

### interlok-core ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.github.mwiede:jsch:0.1.72
- com.thoughtworks.xstream:xstream:1.4.19
- com.zaxxer:HikariCP:5.0.1
- org.bouncycastle:bcmail-jdk15on:1.70
- org.bouncycastle:bcpkix-jdk15on:1.70
- org.bouncycastle:bcprov-jdk15on:1.70
- org.slf4j:slf4j-api:1.7.35
- xerces:xercesImpl:2.12.2

#### Unchanged Dependencies ####
- com.mchange:c3p0:0.9.5.5
- com.sun.activation:jakarta.activation:1.2.2
- com.sun.mail:jakarta.mail:1.6.7
- commons-io:commons-io:2.11.0
- commons-net:commons-net:3.8.0
- io.github.classgraph:classgraph:4.8.116
- jakarta.jms:jakarta.jms-api:2.0.3
- jakarta.validation:jakarta.validation-api:2.0.2
- javax.servlet:javax.servlet-api:4.0.1
- net.jodah:expiringmap:0.5.10
- net.sf.joost:joost:0.9.1
- net.sf.saxon:Saxon-HE:10.6
- org.apache-extras.beanshell:bsh:2.0b6
- org.apache.activemq:activemq-client:5.16.3
- org.apache.commons:commons-collections4:4.4
- org.apache.commons:commons-exec:1.3
- org.apache.commons:commons-lang3:3.12.0
- org.apache.commons:commons-pool2:2.11.1
- org.apache.commons:commons-text:1.9
- org.apache.derby:derby:10.15.2.0
- org.apache.derby:derbytools:10.15.2.0
- org.codehaus.jettison:jettison:1.2
- org.eclipse.jetty.aggregate:jetty-all:9.4.44.v20210927
- org.glassfish.external:opendmk_jdmkrt_jar:1.0-b01-ea
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.glassfish:javax.el:3.0.1-b12
- org.hibernate.javax.persistence:hibernate-jpa-2.1-api:1.0.2.Final
- org.hibernate.validator:hibernate-validator:6.1.7.Final
- org.quartz-scheduler:quartz:2.3.2

### interlok-core-apt ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.19

#### Unchanged Dependencies ####
- jakarta.validation:jakarta.validation-api:2.0.2

### interlok-csv ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.35

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-stax:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- net.sf.supercsv:super-csv:2.4.0

#### Removed Dependencies ####
- com.adaptris:interlok-common:4.3.0-RELEASE

### interlok-csv-json ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.35

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-csv:4.4.0-RELEASE
- com.adaptris:interlok-json:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- org.slf4j:slf4j-api:1.7.35

#### Removed Dependencies ####
- com.adaptris:interlok-common:4.3.0-RELEASE

### interlok-csv-schema ###

#### Initial Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.gilt:gfc-semver_2.11:0.0.5
- org.scala-lang.plugins:scala-continuations-library_2.11:1.0.3
- org.scala-lang:scala-library:2.11.12
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35
- uk.gov.nationalarchives:csv-validator-java-api:1.1.5

### interlok-edi-legacy ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-edi-stream ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- javax.cache:cache-api:1.1.1

### interlok-ehcache ###

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- net.sf.ehcache:ehcache:2.10.9.2

### interlok-elastic-common ###

#### New Dependencies ####
- org.apache.logging.log4j:log4j-api:2.17.1

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-csv:4.4.0-RELEASE
- com.adaptris:interlok-json:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.jayway.jsonpath:json-path:2.7.0
- org.slf4j:slf4j-api:1.7.35
- org.yaml:snakeyaml:1.30

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- commons-collections:commons-collections:3.2.2
- joda-time:joda-time:2.10.13
- net.sf.supercsv:super-csv:2.4.0
- org.apache.commons:commons-csv:1.9.0
- org.apache.httpcomponents:httpclient:4.5.13
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.15.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.15.1

### interlok-elastic-rest ###

#### New Dependencies ####
- org.apache.logging.log4j:log4j-api:2.17.1

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-csv:4.4.0-RELEASE
- com.adaptris:interlok-elastic-common:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.jayway.jsonpath:json-path:2.7.0
- org.slf4j:slf4j-api:1.7.35
- org.yaml:snakeyaml:1.30

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- commons-collections:commons-collections:3.2.2
- joda-time:joda-time:2.10.13
- org.apache.httpcomponents:httpclient:4.5.13
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.15.1
- org.elasticsearch.client:elasticsearch-rest-high-level-client:7.15.1

### interlok-excel ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.apache.commons:commons-compress:1.21
- org.apache.poi:poi-ooxml:4.1.2
- org.apache.poi:poi:4.1.2

### interlok-exec ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.apache.commons:commons-exec:1.3

### interlok-expressions ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.apache-extras.beanshell:bsh:2.0b6

### interlok-failover ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.jgroups:jgroups:4.2.4.Final

### interlok-filesystem ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.apache.tika:tika-core:2.2.1
- org.json:json:20211205
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.hierynomus:smbj:0.11.3
- org.apache.commons:commons-compress:1.21

### interlok-flatfile ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE

### interlok-flyway ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.flywaydb:flyway-core:8.4.3

#### Unchanged Dependencies ####
- commons-collections:commons-collections:3.2.2

### interlok-gcloud-pubsub ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-oauth-gcloud:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.google.cloud:google-cloud-pubsub:1.115.1
- com.google.protobuf:protobuf-java-util:3.19.3
- com.google.protobuf:protobuf-java:3.19.3
- io.grpc:grpc-alts:1.44.0
- io.grpc:grpc-auth:1.44.0
- io.grpc:grpc-netty:1.44.0
- io.grpc:grpc-protobuf:1.44.0
- io.grpc:grpc-stub:1.44.0
- io.netty:netty-codec-http2:4.1.73.Final
- io.netty:netty-codec-http:4.1.73.Final
- io.netty:netty-codec:4.1.73.Final
- io.netty:netty-handler-proxy:4.1.73.Final
- io.netty:netty-handler:4.1.73.Final
- io.netty:netty-transport-native-epoll:4.1.73.Final

#### Unchanged Dependencies ####
- com.google.code.gson:gson:2.8.9
- com.google.guava:guava:31.0.1-jre
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13

### interlok-hpcc ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.apache.commons:commons-exec:1.3
- oro:oro:2.0.8

### interlok-installer ###

#### Updated Dependencies ####
- org.gradle:gradle-tooling-api:7.2

#### Unchanged Dependencies ####
- org.openjfx:javafx-base:11.0.2
- org.openjfx:javafx-controls:11.0.2
- org.openjfx:javafx-fxml:11.0.2
- org.openjfx:javafx-graphics:11.0.2

### interlok-jclouds-aws-sts ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-jclouds-common:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.apache.jclouds.api:sts:2.4.0

### interlok-jclouds-blobstore ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-jclouds-common:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- javax.xml.bind:jaxb-api:2.3.1
- org.apache.jclouds:jclouds-blobstore:2.4.0

### interlok-jclouds-common ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.google.guava:guava:31.0.1-jre
- org.apache.jclouds:jclouds-core:2.4.0

### interlok-jdbc ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.google.guava:guava:31.0.1-jre
- commons-codec:commons-codec:1.15
- org.codehaus.staxmate:stax2:2.1

### interlok-jms-oracleaq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.oracle:ojdbc14:10.2.0.1.0
- com.oracle:oracle-aq:1.0

### interlok-jms-sonicmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE

#### Unchanged Dependencies ####
- com.aurea:sonic-channel:8.5.0
- com.aurea:sonic-client:8.5.0
- com.aurea:sonic-crypto:8.5.0
- com.aurea:sonic-xa:8.5.0
- com.aurea:sonic-xmessage:8.5.0
- org.slf4j:slf4j-api:1.7.32

### interlok-jmx-activemq ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.4.0-RELEASE
- com.thoughtworks.xstream:xstream:1.4.19
- org.slf4j:slf4j-api:1.7.35
- org.springframework:spring-aop:5.3.15
- org.springframework:spring-beans:5.3.15
- org.springframework:spring-context:5.3.15
- org.springframework:spring-core:5.3.15
- org.springframework:spring-jms:5.3.15

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- org.apache.activemq:activemq-client:5.16.3
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-jmx-amqp ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.4.0-RELEASE
- com.thoughtworks.xstream:xstream:1.4.19
- io.netty:netty-buffer:4.1.73.Final
- io.netty:netty-codec-http:4.1.73.Final
- io.netty:netty-codec:4.1.73.Final
- io.netty:netty-common:4.1.73.Final
- io.netty:netty-handler:4.1.73.Final
- io.netty:netty-transport-native-epoll:4.1.73.Final
- io.netty:netty-transport-native-kqueue:4.1.73.Final
- io.netty:netty-transport-native-unix-common:4.1.73.Final
- io.netty:netty-transport:4.1.73.Final
- org.apache.qpid:qpid-jms-client:1.5.0
- org.slf4j:slf4j-api:1.7.35
- org.springframework:spring-aop:5.3.15
- org.springframework:spring-beans:5.3.15
- org.springframework:spring-context:5.3.15
- org.springframework:spring-core:5.3.15
- org.springframework:spring-jms:5.3.15

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.qpid:proton-j:0.33.10
- org.apache.qpid:proton-jms:0.12.2
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-jmx-jms-common ###

#### Updated Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.19
- org.slf4j:slf4j-api:1.7.35
- org.springframework:spring-aop:5.3.15
- org.springframework:spring-beans:5.3.15
- org.springframework:spring-context:5.3.15
- org.springframework:spring-core:5.3.15
- org.springframework:spring-jms:5.3.15

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-jmx-jms-stubs ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.thoughtworks.xstream:xstream:1.4.19
- org.slf4j:slf4j-api:1.7.35
- org.springframework:spring-aop:5.3.15
- org.springframework:spring-beans:5.3.15
- org.springframework:spring-context:5.3.15
- org.springframework:spring-core:5.3.15
- org.springframework:spring-jms:5.3.15

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- javax.management.j2ee:javax.management.j2ee-api:1.1.2
- junit:junit:4.13.2
- org.apache.activemq.protobuf:activemq-protobuf:1.1
- org.apache.activemq:activemq-amqp:5.16.3
- org.apache.activemq:activemq-broker:5.16.3
- org.apache.activemq:activemq-jaas:5.16.3
- org.apache.activemq:activemq-kahadb-store:5.16.3
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-jmx-solace ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.4.0-RELEASE
- com.solacesystems:sol-common:10.13.0
- com.solacesystems:sol-jcsmp:10.13.0
- com.solacesystems:sol-jms:10.13.0
- com.thoughtworks.xstream:xstream:1.4.19
- org.slf4j:slf4j-api:1.7.35
- org.springframework:spring-aop:5.3.15
- org.springframework:spring-beans:5.3.15
- org.springframework:spring-context:5.3.15
- org.springframework:spring-core:5.3.15
- org.springframework:spring-jms:5.3.15

#### Unchanged Dependencies ####
- aopalliance:aopalliance:1.0
- commons-io:commons-io:2.11.0
- commons-lang:commons-lang:2.6
- org.apache.commons:commons-lang3:3.12.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-jmx-sonicmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-jmx-jms-common:4.4.0-RELEASE

#### Unchanged Dependencies ####
- com.aurea:sonic-channel:8.5.0
- com.aurea:sonic-client:8.5.0
- com.aurea:sonic-crypto:8.5.0
- com.aurea:sonic-xa:8.5.0
- com.aurea:sonic-xmessage:8.5.0
- org.slf4j:jcl-over-slf4j:1.7.32
- org.slf4j:slf4j-api:1.7.32

### interlok-jolokia ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE

#### Unchanged Dependencies ####
- org.eclipse.jetty.aggregate:jetty-all:9.4.44.v20210927
- org.jolokia:jolokia-core:1.7.1
- org.jolokia:jolokia-jsr160:1.7.1

### interlok-jq ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- net.thisptr:jackson-jq-extra:1.0.0-preview.20210928
- net.thisptr:jackson-jq:1.0.0-preview.20210928

### interlok-jruby ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.jruby:jruby:9.3.3.0
- org.slf4j:slf4j-api:1.7.35

### interlok-jslt ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.schibsted.spt.data:jslt:0.1.11

### interlok-json ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.13.1
- com.jayway.jsonpath:json-path:2.7.0
- org.json:json:20211205
- org.slf4j:slf4j-api:1.7.35
- xerces:xercesImpl:2.12.2

#### Unchanged Dependencies ####
- com.bazaarvoice.jolt:jolt-core:0.1.5
- com.bazaarvoice.jolt:json-utils:0.1.5
- com.flipkart.zjsonpatch:zjsonpatch:0.4.11
- com.github.everit-org.json-schema:org.everit.json.schema:1.14.0
- com.google.guava:guava:31.0.1-jre
- commons-beanutils:commons-beanutils:1.9.4
- commons-collections:commons-collections:3.2.2
- net.sf.json-lib:json-lib:2.4
- xom:xom:1.3.7

### interlok-json-streaming ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-json:4.4.0-RELEASE
- com.adaptris:interlok-stax:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.github.jsurfer:jsurfer-core:1.6.3
- com.github.jsurfer:jsurfer-gson:1.6.3
- com.github.jsurfer:jsurfer-jackson:1.6.3
- com.github.jsurfer:jsurfer-jsonsimple:1.6.3
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.google.code.gson:gson:2.8.9
- de.odysseus.staxon:staxon:1.3

### interlok-json-web-token ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.bouncycastle:bcpg-jdk15on:1.70
- org.bouncycastle:bcprov-jdk15on:1.70
- org.json:json:20211205
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.12.5
- io.jsonwebtoken:jjwt-api:0.11.2
- io.jsonwebtoken:jjwt-impl:0.11.2
- io.jsonwebtoken:jjwt-jackson:0.11.2

### interlok-jsr107-cache ###

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- javax.cache:cache-api:1.1.1

### interlok-kafka ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- io.netty:netty-codec:4.1.73.Final
- io.netty:netty-handler:4.1.73.Final
- io.netty:netty-transport-native-epoll:4.1.73.Final
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- commons-collections:commons-collections:3.2.2
- org.apache.kafka:kafka-clients:2.4.1
- org.apache.kafka:kafka_2.11:2.4.1

### interlok-kie ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.thoughtworks.xstream:xstream:1.4.19
- org.drools:drools-compiler:7.64.0.Final
- org.drools:drools-core:7.64.0.Final
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- org.apache.commons:commons-collections4:4.4

### interlok-licensing ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.32

### interlok-licensing-demo ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.32

### interlok-logging ###

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-api:2.17.1
- org.apache.logging.log4j:log4j-core:2.17.1

### interlok-mail ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE

#### Unchanged Dependencies ####
- com.sun.mail:jakarta.mail:1.6.7

### interlok-mongodb ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-json:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.mongodb:mongodb-driver:3.12.10

### interlok-mqtt ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- javax.transaction:jta:1.1
- org.apache.httpcomponents:httpclient:4.5.13
- org.eclipse.paho:org.eclipse.paho.client.mqttv3:1.2.5

### interlok-msmq-javonet ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.javonet:javonet:1.4-hf15

### interlok-nats ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- io.nats:jnats:2.13.2

### interlok-oauth-azure ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.nimbusds:nimbus-jose-jwt:9.16.1
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.microsoft.azure:adal4j:1.6.7
- net.minidev:json-smart:2.4.7

### interlok-oauth-gcloud ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.google.auth:google-auth-library-oauth2-http:1.4.0
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.google.guava:guava:31.0.1-jre
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13

### interlok-oauth-generic ###

#### Updated Dependencies ####
- com.adaptris:interlok-apache-http:4.4.0-RELEASE
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.jayway.jsonpath:json-path:2.7.0
- org.slf4j:slf4j-api:1.7.35

### interlok-oauth-salesforce ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- org.apache.httpcomponents:httpclient:4.5.13

### interlok-okhttp ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.squareup.okhttp3:okhttp:4.9.3
- org.slf4j:slf4j-api:1.7.35

### interlok-pdf ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- net.sf.cssbox:pdf2dom:2.0.1
- org.apache.pdfbox:fontbox:2.0.25
- org.apache.pdfbox:pdfbox-tools:2.0.25
- org.apache.pdfbox:pdfbox:2.0.25
- org.apache.xmlgraphics:fop:2.7
- org.slf4j:slf4j-api:1.7.35
- xerces:xercesImpl:2.12.2

#### Unchanged Dependencies ####
- com.google.guava:guava:31.0.1-jre
- commons-io:commons-io:2.11.0

### interlok-pgp ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.bouncycastle:bcpg-jdk15on:1.70
- org.bouncycastle:bcprov-jdk15on:1.70
- org.slf4j:slf4j-api:1.7.35

### interlok-profiler ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.apache.commons:commons-math3:3.6.1
- org.aspectj:aspectjrt:1.9.7
- org.aspectj:aspectjtools:1.9.7
- org.aspectj:aspectjweaver:1.9.7

### interlok-proxy ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.4.0-RELEASE
- com.adaptris:interlok-client:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.apache.httpcomponents.client5:httpclient5:5.1.2

### interlok-rabbitmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.rabbitmq:amqp-client:5.14.1
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

### interlok-rest-base ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.4.0-RELEASE
- com.adaptris:interlok-client:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE

### interlok-rest-cluster ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.4.0-RELEASE
- com.adaptris:interlok-client:4.4.0-RELEASE
- com.adaptris:interlok-cluster-manager:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-rest-base:4.4.0-RELEASE

### interlok-rest-health-check ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.4.0-RELEASE
- com.adaptris:interlok-client:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-rest-base:4.4.0-RELEASE

### interlok-rest-metrics-jvm ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.4.0-RELEASE
- com.adaptris:interlok-client:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-rest-base:4.4.0-RELEASE
- io.micrometer:micrometer-core:1.8.2

#### Unchanged Dependencies ####
- io.github.mweirauch:micrometer-jvm-extras:0.2.2

### interlok-rest-metrics-profiler ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.4.0-RELEASE
- com.adaptris:interlok-client:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-profiler:4.4.0-RELEASE
- com.adaptris:interlok-rest-base:4.4.0-RELEASE
- com.adaptris:interlok-rest-metrics-jvm:4.4.0-RELEASE

### interlok-rest-provider-datadog ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.4.0-RELEASE
- com.adaptris:interlok-client:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-rest-base:4.4.0-RELEASE
- com.adaptris:interlok-rest-metrics-jvm:4.4.0-RELEASE
- io.micrometer:micrometer-registry-datadog:1.8.2

### interlok-rest-provider-prometheus ###

#### Updated Dependencies ####
- com.adaptris:interlok-client-jmx:4.4.0-RELEASE
- com.adaptris:interlok-client:4.4.0-RELEASE
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-rest-base:4.4.0-RELEASE
- com.adaptris:interlok-rest-metrics-jvm:4.4.0-RELEASE
- io.micrometer:micrometer-registry-prometheus:1.8.2

### interlok-sap ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- org.apache.ant:ant:1.10.12
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.sap:sapidoc3:3.0.12
- com.sap:sapjco3:3.0.13

### interlok-service-tester ###

#### New Dependencies ####
- commons-io:commons-io:2.11.0

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-varsub:4.4.0-RELEASE
- com.adaptris:interlok-xinclude:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-service-tester-json ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-service-tester:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.jayway.jsonpath:json-path:2.7.0
- org.json:json:20211205
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.skyscreamer:jsonassert:1.5.0

### interlok-service-tester-wiremock ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-service-tester:4.4.0-RELEASE
- com.fasterxml.jackson.core:jackson-annotations:2.13.1
- com.fasterxml.jackson.core:jackson-core:2.13.1
- com.fasterxml.jackson.core:jackson-databind:2.13.1
- com.github.tomakehurst:wiremock-jre8:2.32.0
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.google.guava:guava:31.0.1-jre

### interlok-service-tester-xml ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-service-tester:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- xmlunit:xmlunit:1.6

### interlok-solace ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.solacesystems:sol-common:10.13.0
- com.solacesystems:sol-jcsmp:10.13.0
- com.solacesystems:sol-jms:10.13.0
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- net.jodah:expiringmap:0.5.10

### interlok-sshtunnel ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.github.mwiede:jsch:0.1.72
- org.slf4j:slf4j-api:1.7.35

### interlok-stax ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-stubs ###

#### Updated Dependencies ####
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- junit:junit:4.13.2

### interlok-swift ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.prowidesoftware:pw-swift-core:SRU2021-9.2.11
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

### interlok-tibco ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.tibco:tibjms:6.3.0
- com.tibco:tibrv:7.5.1

### interlok-triggered ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-varsub ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE

### interlok-vcs-git ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.github.mwiede:jsch:0.1.72
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- commons-codec:commons-codec:1.15
- commons-lang:commons-lang:2.6
- org.apache.httpcomponents:httpclient:4.5.13
- org.eclipse.jgit:org.eclipse.jgit.ssh.jsch:5.13.0.202109080827-r
- org.eclipse.jgit:org.eclipse.jgit:5.13.0.202109080827-r

### interlok-webservice-cxf ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- org.apache.cxf:cxf-rt-frontend-jaxws:3.5.0
- org.apache.cxf:cxf-rt-transports-http:3.5.0
- org.slf4j:slf4j-api:1.7.35

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
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.ibm.mq:com.ibm.mq.allclient:9.2.4.0
- org.slf4j:jcl-over-slf4j:1.7.35
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- org.apache.geronimo.specs:geronimo-j2ee-connector_1.6_spec:1.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1

### interlok-xa-activemq ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- com.adaptris:interlok-xa-jms:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-xa-atomikos ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- com.adaptris:interlok-xa-jms:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.atomikos:transactions-jms:3.8.0
- org.awaitility:awaitility:4.1.1

### interlok-xa-jms ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

### interlok-xa-solace ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- com.adaptris:interlok-solace:4.4.0-RELEASE
- com.adaptris:interlok-xa-jms:4.4.0-RELEASE
- com.solacesystems:sol-common:10.13.0
- com.solacesystems:sol-jcsmp:10.13.0
- com.solacesystems:sol-jms:10.13.0
- org.slf4j:slf4j-api:1.7.35

### interlok-xa-tibco ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- com.adaptris:interlok-tibco:4.4.0-RELEASE
- com.adaptris:interlok-xa-jms:4.4.0-RELEASE
- org.slf4j:slf4j-api:1.7.35

#### Unchanged Dependencies ####
- com.tibco:tibjms:6.3.0
- com.tibco:tibrv:7.5.1

### interlok-xa-wmq ###

#### Updated Dependencies ####
- com.adaptris:interlok-core-apt:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE
- com.adaptris:interlok-webspheremq:4.4.0-RELEASE
- com.adaptris:interlok-xa-jms:4.4.0-RELEASE
- com.ibm.mq:com.ibm.mq.allclient:9.2.4.0
- org.slf4j:slf4j-api:1.7.35

### interlok-xinclude ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE

### interlok-xml-security ###

#### Updated Dependencies ####
- com.adaptris:interlok-common:4.4.0-RELEASE
- com.adaptris:interlok-core:4.4.0-RELEASE
- com.adaptris:interlok-licensing:4.4.0-RELEASE

#### Unchanged Dependencies ####
- iaik:iaik-cms:4.0
- iaik:iaik-jce:3.16
- iaik:iaik-xsect:1.11
- org.slf4j:slf4j-api:1.7.32
