## Version 3.8.0-RELEASE ##

### adaptris-saxon-extensions ###

#### Unchanged Dependencies ####
- net.sf.saxon:Saxon-HE:9.8.0-4
- org.apache.httpcomponents:httpclient:4.5.3
- org.slf4j:jcl-over-slf4j:1.7.25
- org.slf4j:slf4j-api:1.7.25

### interlok-actional-interceptor ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.aurea.actional.agent.sdk:actional-plugmaker:10.0112
- com.aurea.actional.agent.sdk:actional-sdk:10.0112

### interlok-actional-stabiliser ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.aurea:actional-sdk:8.2
- com.aurea:actional-soap-sdk:8.2
- com.aurea:actional-taskapi:8.2
- javax.xml:jaxrpc-api:1.1
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.axis:axis:1.4
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12
- wsdl4j:wsdl4j:1.6.2

### interlok-activemq ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.fasterxml.jackson.core:jackson-core:2.9.6
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- com.google.guava:guava:26.0-jre
- org.apache.activemq:activemq-amqp:5.15.4
- org.apache.activemq:activemq-client:5.15.4
- org.apache.activemq:activemq-jaas:5.15.4
- org.apache.activemq:activemq-kahadb-store:5.15.4
- org.apache.activemq:activemq-mqtt:5.15.4
- org.apache.activemq:activemq-spring:5.15.4
- org.apache.activemq:activemq-stomp:5.15.4
- org.springframework:spring-beans:4.3.18.RELEASE
- org.springframework:spring-context:4.3.18.RELEASE

#### Unchanged Dependencies ####
- org.apache.activemq.protobuf:activemq-protobuf:1.1
- org.apache.activemq:activemq-broker:5.15.2

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-amqp ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.rabbitmq.jms:rabbitmq-jms:1.9.0
- com.rabbitmq:amqp-client:5.3.0
- org.apache.qpid:proton-j:0.28.1
- org.apache.qpid:proton-jms:0.12.2
- org.apache.qpid:qpid-amqp-1-0-client-jms:0.32
- org.apache.qpid:qpid-client:6.3.2
- org.apache.qpid:qpid-jms-client:0.35.0
- org.slf4j:slf4j-api:1.7.25

### interlok-apache-http ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- org.apache.httpcomponents:httpclient:4.5.6

### interlok-as2 ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.adaptris:interlok-varsub:3.8.0-RELEASE
- javax.servlet:javax.servlet-api:3.1.0
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.derby:derby:10.8.2.2
- org.apache.velocity:velocity:1.7
- org.bouncycastle:bcmail-jdk15on:1.60
- org.bouncycastle:bcpkix-jdk15on:1.60
- org.bouncycastle:bcprov-jdk15on:1.60
- org.eclipse.jetty.aggregate:jetty-all:9.4.1.v20170120
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-as400 ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- net.sf.jt400:jt400:9.1
- net.sf:cb2xml:0.92
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-licensing-stub:3.7.3-RELEASE
- com.adaptris:adp-licensing:3.7.3-RELEASE
- com.adaptris:adp-stubs:3.7.3-RELEASE

### interlok-auth-pe ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- com.google.code.gson:gson:2.6.2
- com.squareup.okhttp:logging-interceptor:2.7.5
- com.squareup.okhttp:okhttp:2.7.5
- io.swagger:swagger-annotations:1.5.9
- joda-time:joda-time:2.9.3
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-core:2.1.0-beta.121
- org.slf4j:jcl-over-slf4j:1.7.24
- org.slf4j:slf4j-api:1.7.24
- org.slf4j:slf4j-log4j12:1.7.24

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-stubs:3.7.3-RELEASE

### interlok-aws-common ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Unchanged Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.149
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-aws-s3 ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.149
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-aws-sns ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.149
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-aws-sqs ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-aws-common:3.8.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- org.apache.httpcomponents:httpclient:4.5.6

#### Unchanged Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.0.4
- com.amazonaws:aws-java-sdk-sqs:1.11.149
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-boot ###

#### Unchanged Dependencies ####
- junit:junit:4.11
- org.springframework.boot:spring-boot-loader:1.5.7.RELEASE

### interlok-cassandra ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.datastax.cassandra:cassandra-driver-core:3.0.0
- com.datastax.cassandra:cassandra-driver-mapping:3.0.0
- org.slf4j:slf4j-api:1.7.25

### interlok-cirrus-db ###

#### Initial Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.mchange:c3p0:0.9.5.2
- com.thoughtworks.xstream:xstream:1.4.7
- commons-collections:commons-collections:3.2.2
- commons-dbcp:commons-dbcp:1.4
- commons-io:commons-io:2.4
- commons-lang:commons-lang:2.6
- junit:junit:4.11
- log4j:log4j:1.2.17
- mysql:mysql-connector-java:5.1.25
- org.apache.velocity:velocity:1.7
- org.flywaydb:flyway-core:4.2.0
- org.hibernate:hibernate-c3p0:4.3.7.Final
- org.hibernate:hibernate-core:4.3.7.Final
- org.hibernate:hibernate-entitymanager:4.3.7.Final
- org.hibernate:hibernate-validator:4.3.2.Final
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-cirrus-db-webapp ###

#### Initial Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.mchange:c3p0:0.9.5.2
- com.thoughtworks.xstream:xstream:1.4.7
- commons-collections:commons-collections:3.2.2
- commons-dbcp:commons-dbcp:1.4
- commons-io:commons-io:2.4
- commons-lang:commons-lang:2.6
- junit:junit:4.11
- log4j:log4j:1.2.17
- mysql:mysql-connector-java:5.1.25
- org.apache.velocity:velocity:1.7
- org.flywaydb:flyway-core:4.2.0
- org.hibernate:hibernate-c3p0:4.3.7.Final
- org.hibernate:hibernate-core:4.3.7.Final
- org.hibernate:hibernate-entitymanager:4.3.7.Final
- org.hibernate:hibernate-validator:4.3.2.Final
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-cirrus-services ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.mchange:c3p0:0.9.5.2
- commons-collections:commons-collections:3.2.2
- commons-dbcp:commons-dbcp:1.4
- commons-io:commons-io:2.4
- commons-lang:commons-lang:2.6
- junit:junit:4.11
- log4j:log4j:1.2.17
- mysql:mysql-connector-java:5.1.25
- org.apache.velocity:velocity:1.7
- org.flywaydb:flyway-core:4.2.0
- org.hibernate:hibernate-c3p0:4.3.7.Final
- org.hibernate:hibernate-core:4.3.7.Final
- org.hibernate:hibernate-entitymanager:4.3.7.Final
- org.hibernate:hibernate-validator:4.3.2.Final
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-client ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:interlok-common:3.7.3-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.slf4j:jcl-over-slf4j:1.7.5
- org.slf4j:slf4j-log4j12:1.7.5

### interlok-client-jmx ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-client:3.8.0-RELEASE
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:interlok-common:3.7.3-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.slf4j:jcl-over-slf4j:1.7.5
- org.slf4j:slf4j-log4j12:1.7.5

### interlok-common ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE

#### Updated Dependencies ####
- org.eclipse.jetty.aggregate:jetty-all:9.4.11.v20180605

#### Unchanged Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.10
- commons-collections:commons-collections:3.2.2
- commons-io:commons-io:2.4
- commons-lang:commons-lang:2.6
- commons-net:commons-net:3.3
- commons-pool:commons-pool:1.6
- javax.servlet:javax.servlet-api:3.1.0
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.slf4j:jcl-over-slf4j:1.7.25
- org.slf4j:jul-to-slf4j:1.7.25
- org.slf4j:slf4j-api:1.7.25
- org.slf4j:slf4j-log4j12:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE

### interlok-config-conditional ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-expressions:3.8.0-RELEASE

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE
- org.apache.commons:commons-compress:1.17
- org.json:json:20160810

### interlok-container ###

#### Unchanged Dependencies ####
- org.glassfish.external:opendmk_jdmkrt_jar:1.0-b01-ea
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea

### interlok-core ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.icegreen:greenmail:1.4.0
- com.jcraft:jsch:0.1.54
- com.mchange:c3p0:0.9.5.2
- com.sun.mail:javax.mail:1.6.1
- com.thoughtworks.xstream:xstream:1.4.10
- commons-collections:commons-collections:3.2.2
- commons-io:commons-io:2.6
- commons-lang:commons-lang:2.6
- commons-net:commons-net:3.6
- commons-pool:commons-pool:1.6
- io.github.lukehutch:fast-classpath-scanner:2.9.4
- javax.activation:activation:1.1.1
- javax.el:javax.el-api:2.2.4
- javax.servlet:javax.servlet-api:3.1.0
- javax.validation:validation-api:1.0.0.GA
- javax.xml.bind:jaxb-api:2.3.0
- junit:junit:4.11
- log4j:log4j:1.2.17
- mysql:mysql-connector-java:5.1.40
- net.jodah:expiringmap:0.5.8
- net.sf.joost:joost:0.9.1
- net.sf.saxon:Saxon-HE:9.7.0-20
- org.apache.activemq.protobuf:activemq-protobuf:1.1
- org.apache.activemq:activemq-broker:5.15.2
- org.apache.activemq:activemq-client:5.15.2
- org.apache.activemq:activemq-jaas:5.15.2
- org.apache.activemq:activemq-kahadb-store:5.15.2
- org.apache.commons:commons-exec:1.3
- org.apache.commons:commons-lang3:3.7
- org.apache.derby:derby:10.14.2.0
- org.apache.logging.log4j:log4j-1.2-api:2.9.1
- org.apache.logging.log4j:log4j-api:2.9.1
- org.apache.logging.log4j:log4j-core:2.9.1
- org.apache.velocity:velocity:1.7
- org.bouncycastle:bcmail-jdk15on:1.60
- org.bouncycastle:bcpkix-jdk15on:1.60
- org.bouncycastle:bcprov-jdk15on:1.60
- org.codehaus.jettison:jettison:1.2
- org.eclipse.jetty.aggregate:jetty-all:9.4.11.v20180605
- org.glassfish.external:opendmk_jdmkrt_jar:1.0-b01-ea
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.hibernate.javax.persistence:hibernate-jpa-2.1-api:1.0.0.Final
- org.hibernate:hibernate-validator:4.3.2.Final
- org.jruby:jruby-complete:9.1.13.0
- org.mockftpserver:MockFtpServer:2.4-MDTM
- org.mockito:mockito-all:1.9.5
- org.quartz-scheduler:quartz:2.2.3
- org.slf4j:jcl-over-slf4j:1.7.25
- org.slf4j:jul-to-slf4j:1.7.25
- org.slf4j:slf4j-api:1.7.25
- org.slf4j:slf4j-log4j12:1.7.25
- oro:oro:2.0.8
- xerces:xercesImpl:2.12.0

### interlok-core-apt ###

#### Initial Dependencies ####
- com.thoughtworks.xstream:xstream:1.4.10
- commons-collections:commons-collections:3.2.2
- commons-lang:commons-lang:2.6
- javax.validation:validation-api:1.0.0.GA
- junit:junit:4.11
- org.apache.velocity:velocity:1.7
- org.hibernate:hibernate-validator:4.3.2.Final

### interlok-csv ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stax:3.8.0-RELEASE
- net.sf.supercsv:super-csv:2.4.0
- org.apache.commons:commons-csv:1.5
- org.slf4j:slf4j-api:1.7.25

### interlok-csv-json ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-csv:3.8.0-RELEASE
- com.adaptris:interlok-json:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.9.6

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-json:3.7.3-RELEASE
- com.adaptris:adp-simple-csv:3.7.3-RELEASE

### interlok-drools ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.antlr:antlr-runtime:3.3
- org.antlr:antlr-runtime:3.3
- org.antlr:antlr:3.3
- org.apache.velocity:velocity:1.7
- org.drools:drools-compiler:5.6.0.Final
- org.drools:drools-core:5.6.0.Final
- org.drools:drools-decisiontables:5.6.0.Final
- org.drools:drools-jsr94:5.6.0.Final
- org.mockito:mockito-all:1.9.5
- org.ow2.asm:asm-all:4.1
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-edi-legacy ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- org.slf4j:slf4j-api:1.7.25

### interlok-edi-stream ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- org.slf4j:slf4j-api:1.7.25

### interlok-ehcache ###

#### Initial Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- net.sf.ehcache:ehcache:2.10.5
- org.slf4j:slf4j-api:1.7.25

### interlok-elastic-search ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-csv:3.8.0-RELEASE

#### Updated Dependencies ####
- com.jayway.jsonpath:json-path:2.4.0

#### Unchanged Dependencies ####
- org.elasticsearch:elasticsearch:2.3.5
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-simple-csv:3.7.3-RELEASE

### interlok-es-rest ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-csv:3.8.0-RELEASE
- com.jayway.jsonpath:json-path:2.4.0
- joda-time:joda-time:2.10
- org.apache.commons:commons-compress:1.17
- org.elasticsearch.client:elasticsearch-rest-client-sniffer:6.3.2
- org.elasticsearch.client:elasticsearch-rest-high-level-client:6.3.2
- org.json:json:20180130
- org.slf4j:slf4j-api:1.7.25

### interlok-es5 ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-csv:3.8.0-RELEASE

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- com.jayway.jsonpath:json-path:2.4.0

#### Unchanged Dependencies ####
- io.netty:netty-all:4.1.9.Final
- org.elasticsearch.plugin:transport-netty4-client:5.2.2
- org.elasticsearch:elasticsearch:5.2.2
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-simple-csv:3.7.3-RELEASE

### interlok-excel ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- commons-io:commons-io:2.4
- commons-lang:commons-lang:2.6
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.poi:poi-ooxml:3.10-FINAL
- org.apache.poi:poi:3.10-FINAL
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-expressions ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- org.apache.commons:commons-compress:1.17
- org.beanshell:bsh:2.1b5
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-failover ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-stubs:3.7.3-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-filesystem ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- org.json:json:20180130

#### Unchanged Dependencies ####
- org.apache.commons:commons-compress:1.17
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE
- org.apache.httpcomponents:httpclient:4.5.6

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-oauth-gcloud:3.8.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- com.google.cloud:google-cloud-pubsub:1.38.0
- com.google.guava:guava:26.0-jre

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-hornetq ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.hornetq:hornetq-commons:2.3.1.Final
- org.hornetq:hornetq-core-client:2.3.1.Final
- org.hornetq:hornetq-jms-client:2.3.1.Final
- org.hornetq:hornetq-jms-server:2.3.1.Final
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-hpcc ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- org.apache.commons:commons-exec:1.3
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-interfax ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- interfax:interfax:1.0
- javax.xml.soap:saaj-api:1.3.5
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.axis:axis-jaxrpc:1.4
- org.apache.axis:axis:1.4
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-ironmq ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.google.code.gson:gson:2.2.4
- io.iron.ironmq:ironmq:3.0.5
- org.quartz-scheduler:quartz:2.2.1
- org.slf4j:slf4j-api:1.7.25

### interlok-jclouds-blobstore ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.google.guava:guava:26.0-jre

#### Unchanged Dependencies ####
- org.apache.jclouds:jclouds-blobstore:2.1.0
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-jetty-auth-realm ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.googlecode.json-simple:json-simple:1.1.1
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.commons:commons-collections4:4.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.10.19
- org.powermock:powermock-api-mockito:1.6.5
- org.powermock:powermock-module-junit4:1.6.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-jms-oracleaq ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.oracle:ojdbc14:10.2.0.1.0
- com.oracle:oracle-aq:1.0
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-jms-sonicmq ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.aurea:sonic-channel:8.5.0
- com.aurea:sonic-client:8.5.0
- com.aurea:sonic-crypto:8.5.0
- com.aurea:sonic-xa:8.5.0
- com.aurea:sonic-xmessage:8.5.0
- com.aurea:sonicmq-mfcontext:8.5.0
- com.aurea:sonicmq-mgmt-client:8.5.0
- com.aurea:sonicmq-mgmt-config:8.5.0
- com.aurea:sonicmq-sonic-mgmt-client:8.5.0
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-jmx-jms ###

#### Initial Dependencies ####
- aopalliance:aopalliance:1.0
- com.aurea:sonic-channel:8.5.0
- com.aurea:sonic-client:8.5.0
- com.aurea:sonic-crypto:8.5.0
- com.aurea:sonic-xa:8.5.0
- com.aurea:sonic-xmessage:8.5.0
- com.rabbitmq.jms:rabbitmq-jms:1.6.0
- com.rabbitmq:amqp-client:4.0.2
- com.solacesystems:sol-common:10.1.1
- com.solacesystems:sol-jcsmp:10.1.1
- com.solacesystems:sol-jms:10.1.1
- com.thoughtworks.xstream:xstream:1.4.10
- commons-lang:commons-lang:2.6
- org.apache.activemq:activemq-client:5.15.4
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.qpid:proton-j:0.17.0
- org.apache.qpid:proton-jms:0.12.1
- org.apache.qpid:qpid-jms-client:0.11.1
- org.codehaus.jettison:jettison:1.2
- org.glassfish.external:opendmk_jmxremote_optional_jar:1.0-b01-ea
- org.slf4j:jcl-over-slf4j:1.7.25
- org.slf4j:slf4j-api:1.7.25
- org.slf4j:slf4j-log4j12:1.7.25
- org.springframework:spring-aop:4.3.18.RELEASE
- org.springframework:spring-beans:4.3.18.RELEASE
- org.springframework:spring-context:4.3.18.RELEASE
- org.springframework:spring-core:4.3.18.RELEASE
- org.springframework:spring-jms:4.3.18.RELEASE

### interlok-jq ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- net.thisptr:jackson-jq:0.0.9

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-jruby ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- org.jruby:jruby:9.2.0.0

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-json ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.bazaarvoice.jolt:jolt-core:0.1.1
- com.bazaarvoice.jolt:json-utils:0.1.1
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.9.6
- com.google.guava:guava:26.0-jre
- com.jayway.jsonpath:json-path:2.4.0
- commons-beanutils:commons-beanutils:1.9.3
- commons-collections:commons-collections:3.2.2
- net.sf.json-lib:json-lib:2.4
- org.everit.json:org.everit.json.schema:1.5.1
- org.json:json:20180130
- org.slf4j:slf4j-api:1.7.25
- xerces:xercesImpl:2.12.0
- xom:xom:1.2.5

### interlok-jsr107-cache ###

#### Initial Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- javax.cache:cache-api:1.1.0
- org.slf4j:slf4j-api:1.7.25

### interlok-kafka ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.kafka:kafka-clients:0.9.0.1
- org.apache.kafka:kafka_2.11:0.9.0.1
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-legacyhttp ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.24
- org.slf4j:slf4j-api:1.7.24
- org.slf4j:slf4j-log4j12:1.7.24

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-stubs:3.7.3-RELEASE

### interlok-licensing ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-logging ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE

#### Unchanged Dependencies ####
- junit:junit:4.11
- org.apache.logging.log4j:log4j-api:2.9.1
- org.apache.logging.log4j:log4j-core:2.9.1

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE

### interlok-mongodb ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-json:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- org.mongodb:mongodb-driver:3.8.0

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-json:3.7.3-RELEASE

### interlok-mqtt ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.6

#### Unchanged Dependencies ####
- javax.transaction:jta:1.1
- org.eclipse.paho:org.eclipse.paho.client.mqttv3:1.2.0
- org.slf4j:jcl-over-slf4j:1.7.25
- org.slf4j:slf4j-api:1.7.25
- org.slf4j:slf4j-log4j12:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE
- com.atomikos:transactions-jms:3.8.0

### interlok-msmq ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.inzoom:21100718:1.5.2.1
- com.inzoom:izmcomjni:1.5.2.1
- com.inzoom:izmjnicom:1.5.2.1
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-msmq-javonet ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.javonet:javonet:1.4-hf15
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-new-relic ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-profiler:3.8.0-RELEASE
- com.newrelic.agent.java:newrelic-api:3.12.0
- commons-jexl:commons-jexl:1.1
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-oauth-azure ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.microsoft.azure:adal4j:1.6.0
- net.minidev:json-smart:2.3

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-oauth-gcloud ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.9.6
- com.google.auth:google-auth-library-oauth2-http:0.10.0
- com.google.guava:guava:26.0-jre
- org.apache.httpcomponents:httpclient:4.5.6

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-oauth-salesforce ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- org.apache.httpcomponents:httpclient:4.5.6

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-oftp ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-pdf ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
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
- org.apache.xmlgraphics:fop:1.1
- org.apache.xmlgraphics:xmlgraphics-commons:1.5
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-profiler ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- junit:junit:4.12
- log4j:log4j:1.2.17
- org.aspectj:aspectjrt:1.9.1
- org.aspectj:aspectjtools:1.9.1
- org.aspectj:aspectjweaver:1.9.1
- org.slf4j:jcl-over-slf4j:1.7.25
- org.slf4j:slf4j-api:1.7.25
- org.slf4j:slf4j-log4j12:1.7.25

### interlok-profiler-failover ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-profiler:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- net.sf.ehcache:ehcache-core:2.6.8
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-reliable-messaging ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.derby:derby:10.10.1.1
- org.apache.geronimo.specs:geronimo-servlet_3.0_spec:1.0
- org.apache.velocity:velocity:1.7
- org.eclipse.jetty.aggregate:jetty-all:8.1.14.v20131031
- org.quartz-scheduler:quartz:2.2.1
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-salesforce ###

#### Initial Dependencies ####
- c3p0:c3p0:0.9.1.2
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.mchange:mchange-commons-java:0.2.2
- com.sforce:salesforce-api:3.0
- commons-io:commons-io:2.4
- commons-lang:commons-lang:2.6
- junit:junit:4.11
- log4j:log4j:1.2.17
- mysql:mysql-connector-java:5.1.25
- org.apache.axis:axis-jaxrpc:1.4
- org.apache.axis:axis:1.4
- org.apache.derby:derby:10.8.2.2
- org.apache.velocity:velocity:1.7
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12
- org.springframework:spring-jdbc:4.3.2.RELEASE
- xalan:serializer:2.7.1
- xalan:xalan:2.7.1

### interlok-sap ###

#### Initial Dependencies ####
- cglib:cglib-nodep:2.2.2
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.sap:sapidoc:3.0.12
- com.sap:sapjco:3.0.12
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.hamcrest:hamcrest-core:1.3
- org.jmock:jmock-junit4:2.6.0
- org.jmock:jmock-legacy:2.6.0
- org.jmock:jmock:2.6.0
- org.objenesis:objenesis:2.0
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-schema ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.thaiopensource:jing:20091111
- com.thoughtworks.xstream:xstream:1.4.10
- commons-cli:commons-cli:20040117.000000
- io.github.lukehutch:fast-classpath-scanner:2.9.4
- junit:junit:3.8.1
- log4j:log4j:1.2.17
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12
- xmlpull:xmlpull:1.1.3.1

### interlok-service-tester ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.adaptris:interlok-varsub:3.8.0-RELEASE
- com.adaptris:interlok-xinclude:3.8.0-RELEASE
- org.apache.ant:ant-junit:1.10.5

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- com.github.tomakehurst:wiremock:1.58
- org.skyscreamer:jsonassert:1.5.0
- org.slf4j:slf4j-api:1.7.25
- xmlunit:xmlunit:1.6

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-stubs:3.7.3-RELEASE
- com.adaptris:adp-varsub:3.7.3-RELEASE
- com.adaptris:adp-xinclude:3.7.3-RELEASE

### interlok-shell ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE
- org.bouncycastle:bcpkix-jdk15on:1.60
- org.bouncycastle:bcprov-jdk15on:1.60
- org.codehaus.groovy:groovy-all:2.5.1

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- org.apache.sshd:sshd-core:0.11.0
- org.apache.sshd:sshd-pam:0.11.0
- org.crashub:crash.cli:1.3.2
- org.crashub:crash.connectors.ssh:1.3.2
- org.crashub:crash.shell:1.3.2
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-socket ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-solace ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.solacesystems:sol-common:7.2.1.148
- com.solacesystems:sol-jcsmp:7.2.1.148
- com.solacesystems:sol-jms:7.2.1.148
- commons-lang:commons-lang:2.6
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-sshtunnel ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- com.jcraft:jsch:0.1.54
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-stackify ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-profiler:3.8.0-RELEASE
- com.fasterxml.jackson.core:jackson-core:2.9.6
- com.fasterxml.jackson.core:jackson-databind:2.9.6
- com.stackify:stackify-metrics:1.1.7
- org.slf4j:slf4j-api:1.7.25

### interlok-stax ###

#### New Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core:3.7.3-RELEASE

### interlok-stubs ###

#### Initial Dependencies ####
- com.adaptris:interlok-core:3.8.0-RELEASE

### interlok-swift ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.prowidesoftware.swift:swift:7.0
- commons-io:commons-io:2.4
- commons-lang:commons-lang:2.6
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-swiftmq ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.sun.mail:javax.mail:1.5.6
- com.swiftmq:amqp:9.3.1
- com.swiftmq:swiftmq:9.3.1
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.activemq.protobuf:activemq-protobuf:1.1
- org.apache.activemq:activemq-amqp:5.15.2
- org.apache.activemq:activemq-broker:5.15.2
- org.apache.activemq:activemq-client:5.15.2
- org.apache.activemq:activemq-jaas:5.15.2
- org.apache.activemq:activemq-kahadb-store:5.15.2
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-tibco ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.tibco:tibjms:6.3.0
- com.tibco:tibrv:7.5.1
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-triggered ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-variodoc ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE

#### Unchanged Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-licensing-stub:3.7.3-RELEASE
- com.adaptris:adp-licensing:3.7.3-RELEASE
- com.adaptris:adp-stubs:3.7.3-RELEASE

### interlok-varsub ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

### interlok-vcs-command-line ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE

#### Unchanged Dependencies ####
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-stubs:3.7.3-RELEASE

### interlok-vcs-git ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.jcraft:jsch:0.1.54
- commons-lang:commons-lang:2.6
- org.apache.httpcomponents:httpclient:4.5.6
- org.eclipse.jgit:org.eclipse.jgit:4.1.0.201509280440-r
- org.slf4j:slf4j-api:1.7.25

### interlok-vcs-subversion ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- net.java.dev.jna:jna:3.4.0
- org.slf4j:slf4j-api:1.7.25
- org.tigris.subversion:org.tigris.subversion.clientadapter.javahl-win32:1.7.10
- org.tigris.subversion:org.tigris.subversion.clientadapter.javahl-win64:1.7.10
- org.tigris.subversion:org.tigris.subversion.clientadapter.javahl:1.7.10
- org.tigris.subversion:org.tigris.subversion.clientadapter:1.8.6

### interlok-vertx ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

#### Updated Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.hazelcast:hazelcast:3.10.4
- io.vertx:vertx-core:3.5.3
- io.vertx:vertx-hazelcast:3.5.3
- org.slf4j:slf4j-api:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-licensing-stub:3.7.3-RELEASE
- com.adaptris:adp-licensing:3.7.3-RELEASE
- com.adaptris:adp-stubs:3.7.3-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-webservice-cxf ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.cxf:cxf-rt-frontend-jaxws:2.7.7
- org.apache.cxf:cxf-rt-transports-http:2.7.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-webservice-external ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.sun.xml.ws:jaxws-tools:2.2.8
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.cxf:cxf-rt-frontend-jaxws:2.7.7
- org.apache.cxf:cxf-rt-transports-http:2.7.7
- org.mockito:mockito-all:1.9.5
- org.reflections:reflections:0.9.9-RC1
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-webspheremq ###

#### Initial Dependencies ####
- cglib:cglib-nodep:2.2.2
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- com.ibm:mq:6.0.0.0
- com.ibm:mqjms:6.0.0.0
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-j2ee-connector_1.6_spec:1.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.hamcrest:hamcrest-core:1.3
- org.jmock:jmock-junit4:2.6.0
- org.jmock:jmock-legacy:2.6.0
- org.jmock:jmock:2.6.0
- org.mockito:mockito-all:1.9.5
- org.objenesis:objenesis:2.0
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12

### interlok-xa ###

#### New Dependencies ####
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE

#### Unchanged Dependencies ####
- com.atomikos:transactions-jms:3.8.0
- javax.transaction:jta:1.1
- org.slf4j:jcl-over-slf4j:1.7.25
- org.slf4j:slf4j-api:1.7.25
- org.slf4j:slf4j-log4j12:1.7.25

#### Removed Dependencies ####
- com.adaptris:adp-core-apt:3.7.3-RELEASE
- com.adaptris:adp-core:3.7.3-RELEASE
- com.adaptris:adp-licensing:3.7.3-RELEASE

### interlok-xinclude ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE

### interlok-xml-security ###

#### Initial Dependencies ####
- com.adaptris:interlok-common:3.8.0-RELEASE
- com.adaptris:interlok-core-apt:3.8.0-RELEASE
- com.adaptris:interlok-core:3.8.0-RELEASE
- com.adaptris:interlok-licensing-stub:3.8.0-RELEASE
- com.adaptris:interlok-licensing:3.8.0-RELEASE
- com.adaptris:interlok-stubs:3.8.0-RELEASE
- iaik:iaik-cms:4.0
- iaik:iaik-jce:3.16
- iaik:iaik-xsect:1.11
- junit:junit:4.11
- log4j:log4j:1.2.17
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.apache.velocity:velocity:1.7
- org.mockito:mockito-all:1.9.5
- org.slf4j:jcl-over-slf4j:1.7.12
- org.slf4j:slf4j-api:1.7.12
- org.slf4j:slf4j-log4j12:1.7.12
