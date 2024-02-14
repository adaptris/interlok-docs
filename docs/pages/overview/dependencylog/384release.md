## Version 3.8.4 ##

### interlok-activemq ###

#### New Dependencies ####
- com.google.guava:guava:27.1-jre
- org.apache.activemq:activemq-amqp:5.15.9
- org.apache.activemq:activemq-broker:5.15.9
- org.apache.activemq:activemq-client:5.15.9
- org.apache.activemq:activemq-jaas:5.15.9
- org.apache.activemq:activemq-kahadb-store:5.15.9
- org.apache.activemq:activemq-mqtt:5.15.9
- org.apache.activemq:activemq-spring:5.15.9
- org.apache.activemq:activemq-stomp:5.15.9
- org.apache.qpid:proton-j:0.32.0
- org.springframework:spring-beans:4.3.23.RELEASE
- org.springframework:spring-context:4.3.23.RELEASE

#### Updated Dependencies ####
- com.google.guava:guava:27.1-jre *(from 27.0.1-jre)*
- org.apache.activemq:activemq-amqp:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-broker:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-client:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-jaas:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-kahadb-store:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-mqtt:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-spring:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-stomp:5.15.9 *(from 5.15.8)*
- org.apache.qpid:proton-j:0.32.0 *(from 0.31.0)*
- org.springframework:spring-beans:4.3.23.RELEASE *(from 4.3.22.RELEASE)*
- org.springframework:spring-context:4.3.23.RELEASE *(from 4.3.22.RELEASE)*

### interlok-amqp ###

#### New Dependencies ####
- com.rabbitmq:amqp-client:5.6.0
- org.apache.qpid:proton-j:0.32.0
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.rabbitmq:amqp-client:5.6.0 *(from 5.5.2)*
- org.apache.qpid:proton-j:0.32.0 *(from 0.31.0)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-apache-http ###

#### New Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.8

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.8 *(from 4.5.7)*

### interlok-as2 ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-as400 ###

#### New Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.12)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.12)*

#### Removed Dependencies ####
- ~~junit:junit:4.11~~
- ~~log4j:log4j:1.2.17~~
- ~~org.apache.velocity:velocity:1.7~~
- ~~org.mockito:mockito-all:1.9.5~~
- ~~org.slf4j:slf4j-log4j12:1.7.12~~

### interlok-auth-pe ###

#### New Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.24)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.24)*

#### Removed Dependencies ####
- ~~junit:junit:4.11~~
- ~~log4j:log4j:1.2.17~~
- ~~org.apache.velocity:velocity:1.7~~
- ~~org.mockito:mockito-core:2.1.0-beta.121~~
- ~~org.slf4j:slf4j-log4j12:1.7.24~~

### interlok-aws-common ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.508
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.508 *(from 1.11.490)*
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-aws-s3 ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.508
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.508 *(from 1.11.490)*
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-aws-sns ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.508
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.508 *(from 1.11.490)*
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-aws-sqs ###

#### New Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.0.5
- com.amazonaws:aws-java-sdk-sqs:1.11.508
- org.apache.httpcomponents:httpclient:4.5.8
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.0.5 *(from 1.0.4)*
- com.amazonaws:aws-java-sdk-sqs:1.11.508 *(from 1.11.490)*
- org.apache.httpcomponents:httpclient:4.5.8 *(from 4.5.7)*
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-cassandra ###

#### New Dependencies ####
- com.google.guava:guava:27.1-jre
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.google.guava:guava:27.1-jre *(from 27.0.1-jre)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-client ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-client-jmx ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-common ###

#### New Dependencies ####
- org.apache.commons:commons-pool2:2.6.1
- org.eclipse.jetty.aggregate:jetty-all:9.4.15.v20190215
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:jul-to-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

#### Updated Dependencies ####
- org.apache.commons:commons-pool2:2.6.1 *(from 2.6.0)*
- org.eclipse.jetty.aggregate:jetty-all:9.4.15.v20190215 *(from 9.4.14.v20181114)*
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:jul-to-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-log4j12:1.7.26 *(from 1.7.25)*

### interlok-config-conditional ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-core ###

#### New Dependencies ####
- com.icegreen:greenmail:1.5.10
- com.mchange:c3p0:0.9.5.4
- io.github.classgraph:classgraph:4.8.22
- org.apache.activemq:activemq-broker:5.15.9
- org.apache.activemq:activemq-client:5.15.9
- org.apache.activemq:activemq-jaas:5.15.9
- org.apache.activemq:activemq-kahadb-store:5.15.9
- org.apache.commons:commons-pool2:2.6.1
- org.apache.logging.log4j:log4j-1.2-api:2.11.2
- org.apache.logging.log4j:log4j-api:2.11.2
- org.apache.logging.log4j:log4j-core:2.11.2
- org.bouncycastle:bcmail-jdk15on:1.61
- org.bouncycastle:bcpkix-jdk15on:1.61
- org.bouncycastle:bcprov-jdk15on:1.61
- org.eclipse.jetty.aggregate:jetty-all:9.4.15.v20190215
- org.jruby:jruby-complete:9.2.6.0
- org.quartz-scheduler:quartz:2.3.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:jul-to-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

#### Updated Dependencies ####
- com.icegreen:greenmail:1.5.10 *(from 1.5.9)*
- com.mchange:c3p0:0.9.5.4 *(from 0.9.5.3)*
- io.github.classgraph:classgraph:4.8.22 *(from 4.6.13)*
- org.apache.activemq:activemq-broker:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-client:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-jaas:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-kahadb-store:5.15.9 *(from 5.15.8)*
- org.apache.commons:commons-pool2:2.6.1 *(from 2.6.0)*
- org.apache.logging.log4j:log4j-1.2-api:2.11.2 *(from 2.9.1)*
- org.apache.logging.log4j:log4j-api:2.11.2 *(from 2.9.1)*
- org.apache.logging.log4j:log4j-core:2.11.2 *(from 2.9.1)*
- org.bouncycastle:bcmail-jdk15on:1.61 *(from 1.60)*
- org.bouncycastle:bcpkix-jdk15on:1.61 *(from 1.60)*
- org.bouncycastle:bcprov-jdk15on:1.61 *(from 1.60)*
- org.eclipse.jetty.aggregate:jetty-all:9.4.15.v20190215 *(from 9.4.14.v20181114)*
- org.jruby:jruby-complete:9.2.6.0 *(from 9.2.5.0)*
- org.quartz-scheduler:quartz:2.3.1 *(from 2.3.0)*
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:jul-to-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-log4j12:1.7.26 *(from 1.7.25)*

### interlok-csv ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-csv-json ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-drools ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-edi-legacy ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-ehcache ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-elastic-search ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-es-rest ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-es5 ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-excel ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-exec ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-expressions ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-failover ###

#### New Dependencies ####
- org.jgroups:jgroups:4.0.16.Final
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-filesystem ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.google.cloud:google-cloud-pubsub:1.67.0
- com.google.guava:guava:27.1-jre
- org.apache.httpcomponents:httpclient:4.5.8

#### Updated Dependencies ####
- com.google.cloud:google-cloud-pubsub:1.67.0 *(from 1.61.0)*
- com.google.guava:guava:27.1-jre *(from 27.0.1-jre)*
- org.apache.httpcomponents:httpclient:4.5.8 *(from 4.5.7)*

### interlok-hpcc ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-interfax ###

#### New Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.12)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.12)*

#### Removed Dependencies ####
- ~~junit:junit:4.11~~
- ~~log4j:log4j:1.2.17~~
- ~~org.apache.velocity:velocity:1.7~~
- ~~org.mockito:mockito-all:1.9.5~~
- ~~org.slf4j:slf4j-log4j12:1.7.12~~

### interlok-jclouds-blobstore ###

#### New Dependencies ####
- com.google.guava:guava:27.1-jre
- org.apache.jclouds:jclouds-blobstore:2.1.2
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.google.guava:guava:27.1-jre *(from 27.0.1-jre)*
- org.apache.jclouds:jclouds-blobstore:2.1.2 *(from 2.1.1)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-jms-oracleaq ###

#### New Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.12)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.12)*

#### Removed Dependencies ####
- ~~junit:junit:4.11~~
- ~~log4j:log4j:1.2.17~~
- ~~org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1~~
- ~~org.apache.velocity:velocity:1.7~~
- ~~org.mockito:mockito-all:1.9.5~~
- ~~org.slf4j:slf4j-log4j12:1.7.12~~

### interlok-jq ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-jruby ###

#### New Dependencies ####
- org.jruby:jruby:9.2.6.0
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.jruby:jruby:9.2.6.0 *(from 9.2.5.0)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-json ###

#### New Dependencies ####
- com.google.guava:guava:27.1-jre
- org.slf4j:slf4j-api:1.7.26
- xom:xom:1.3.2

#### Updated Dependencies ####
- com.google.guava:guava:27.1-jre *(from 27.0.1-jre)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*
- xom:xom:1.3.2 *(from 1.2.5)*

### interlok-jsr107-cache ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-kafka ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-kie ###

#### New Dependencies ####
- org.apache.commons:commons-collections4:4.3
- org.drools:drools-compiler:7.20.0.Final
- org.drools:drools-core:7.20.0.Final
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.apache.commons:commons-collections4:4.3 *(from 4.2)*
- org.drools:drools-compiler:7.20.0.Final *(from 7.17.0.Final)*
- org.drools:drools-core:7.20.0.Final *(from 7.17.0.Final)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-legacyhttp ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-logging ###

#### New Dependencies ####
- org.apache.logging.log4j:log4j-api:2.11.2
- org.apache.logging.log4j:log4j-core:2.11.2

#### Updated Dependencies ####
- org.apache.logging.log4j:log4j-api:2.11.2 *(from 2.9.1)*
- org.apache.logging.log4j:log4j-core:2.11.2 *(from 2.9.1)*

### interlok-mongodb ###

#### New Dependencies ####
- org.mongodb:mongodb-driver:3.10.1
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.mongodb:mongodb-driver:3.10.1 *(from 3.9.1)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-mqtt ###

#### New Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.8
- org.eclipse.paho:org.eclipse.paho.client.mqttv3:1.2.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.8 *(from 4.5.7)*
- org.eclipse.paho:org.eclipse.paho.client.mqttv3:1.2.1 *(from 1.2.0)*
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-log4j12:1.7.26 *(from 1.7.25)*

### interlok-oauth-azure ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-oauth-gcloud ###

#### New Dependencies ####
- com.google.auth:google-auth-library-oauth2-http:0.15.0
- com.google.guava:guava:27.1-jre
- org.apache.httpcomponents:httpclient:4.5.8
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.google.auth:google-auth-library-oauth2-http:0.15.0 *(from 0.12.0)*
- com.google.guava:guava:27.1-jre *(from 27.0.1-jre)*
- org.apache.httpcomponents:httpclient:4.5.8 *(from 4.5.7)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-oauth-generic ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-oauth-salesforce ###

#### New Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.8
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.8 *(from 4.5.7)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-oftp ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.12)*

#### Removed Dependencies ####
- ~~junit:junit:4.11~~
- ~~log4j:log4j:1.2.17~~
- ~~org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1~~
- ~~org.apache.velocity:velocity:1.7~~
- ~~org.mockito:mockito-all:1.9.5~~
- ~~org.slf4j:jcl-over-slf4j:1.7.12~~
- ~~org.slf4j:slf4j-log4j12:1.7.12~~

### interlok-okhttp ###

#### New Dependencies ####
- com.squareup.okhttp3:okhttp:3.14.0
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.squareup.okhttp3:okhttp:3.14.0 *(from 3.12.1)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-pdf ###

#### New Dependencies ####
- org.apache.pdfbox:fontbox:2.0.14
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.apache.pdfbox:fontbox:2.0.14 *(from 2.0.13)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-profiler ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-service-tester ###

#### New Dependencies ####
- com.github.tomakehurst:wiremock:2.22.0
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.github.tomakehurst:wiremock:2.22.0 *(from 2.20.0)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-shell ###

#### New Dependencies ####
- org.bouncycastle:bcpkix-jdk15on:1.61
- org.bouncycastle:bcprov-jdk15on:1.61
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.bouncycastle:bcpkix-jdk15on:1.61 *(from 1.60)*
- org.bouncycastle:bcprov-jdk15on:1.61 *(from 1.60)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-socket ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-sshtunnel ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-stax ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-stubs ###

#### New Dependencies ####
- com.icegreen:greenmail:1.5.10
- com.mchange:c3p0:0.9.5.4
- io.github.classgraph:classgraph:4.8.22
- org.apache.activemq:activemq-broker:5.15.9
- org.apache.activemq:activemq-client:5.15.9
- org.apache.activemq:activemq-jaas:5.15.9
- org.apache.activemq:activemq-kahadb-store:5.15.9
- org.apache.commons:commons-pool2:2.6.1
- org.apache.logging.log4j:log4j-1.2-api:2.11.2
- org.apache.logging.log4j:log4j-api:2.11.2
- org.apache.logging.log4j:log4j-core:2.11.2
- org.bouncycastle:bcmail-jdk15on:1.61
- org.bouncycastle:bcpkix-jdk15on:1.61
- org.bouncycastle:bcprov-jdk15on:1.61
- org.eclipse.jetty.aggregate:jetty-all:9.4.15.v20190215
- org.jruby:jruby-complete:9.2.6.0
- org.quartz-scheduler:quartz:2.3.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:jul-to-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

#### Updated Dependencies ####
- com.icegreen:greenmail:1.5.10 *(from 1.5.9)*
- com.mchange:c3p0:0.9.5.4 *(from 0.9.5.3)*
- io.github.classgraph:classgraph:4.8.22 *(from 4.6.13)*
- org.apache.activemq:activemq-broker:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-client:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-jaas:5.15.9 *(from 5.15.8)*
- org.apache.activemq:activemq-kahadb-store:5.15.9 *(from 5.15.8)*
- org.apache.commons:commons-pool2:2.6.1 *(from 2.6.0)*
- org.apache.logging.log4j:log4j-1.2-api:2.11.2 *(from 2.9.1)*
- org.apache.logging.log4j:log4j-api:2.11.2 *(from 2.9.1)*
- org.apache.logging.log4j:log4j-core:2.11.2 *(from 2.9.1)*
- org.bouncycastle:bcmail-jdk15on:1.61 *(from 1.60)*
- org.bouncycastle:bcpkix-jdk15on:1.61 *(from 1.60)*
- org.bouncycastle:bcprov-jdk15on:1.61 *(from 1.60)*
- org.eclipse.jetty.aggregate:jetty-all:9.4.15.v20190215 *(from 9.4.14.v20181114)*
- org.jruby:jruby-complete:9.2.6.0 *(from 9.2.5.0)*
- org.quartz-scheduler:quartz:2.3.1 *(from 2.3.0)*
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:jul-to-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-log4j12:1.7.26 *(from 1.7.25)*

### interlok-swift ###

#### New Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.12)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.12)*

#### Removed Dependencies ####
- ~~commons-io:commons-io:2.4~~
- ~~commons-lang:commons-lang:2.6~~
- ~~junit:junit:4.11~~
- ~~log4j:log4j:1.2.17~~
- ~~org.apache.velocity:velocity:1.7~~
- ~~org.mockito:mockito-all:1.9.5~~
- ~~org.slf4j:slf4j-log4j12:1.7.12~~

### interlok-swiftmq ###

#### New Dependencies ####
- org.apache.geronimo.specs:geronimo-j2ee-connector_1.6_spec:1.0
- org.apache.geronimo.specs:geronimo-jms_1.1_spec:1.1.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.12)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.12)*

#### Removed Dependencies ####
- ~~com.sun.mail:javax.mail:1.5.6~~
- ~~junit:junit:4.11~~
- ~~log4j:log4j:1.2.17~~
- ~~org.apache.activemq.protobuf:activemq-protobuf:1.1~~
- ~~org.apache.activemq:activemq-amqp:5.15.2~~
- ~~org.apache.activemq:activemq-broker:5.15.2~~
- ~~org.apache.activemq:activemq-client:5.15.2~~
- ~~org.apache.activemq:activemq-jaas:5.15.2~~
- ~~org.apache.activemq:activemq-kahadb-store:5.15.2~~
- ~~org.apache.velocity:velocity:1.7~~
- ~~org.mockito:mockito-all:1.9.5~~
- ~~org.slf4j:slf4j-log4j12:1.7.12~~

### interlok-tibco ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-triggered ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-variodoc ###

#### New Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.12)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.12)*

#### Removed Dependencies ####
- ~~junit:junit:4.11~~
- ~~log4j:log4j:1.2.17~~
- ~~org.apache.velocity:velocity:1.7~~
- ~~org.mockito:mockito-all:1.9.5~~
- ~~org.slf4j:slf4j-log4j12:1.7.12~~

### interlok-vcs-command-line ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-vcs-git ###

#### New Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.8
- org.eclipse.jgit:org.eclipse.jgit:5.3.0.201903130848-r
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.8 *(from 4.5.7)*
- org.eclipse.jgit:org.eclipse.jgit:5.3.0.201903130848-r *(from 5.2.1.201812262042-r)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-vcs-subversion ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-vertx ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-webservice-cxf ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-webspheremq ###

#### New Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-xa ###

#### New Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

#### Updated Dependencies ####
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-log4j12:1.7.26 *(from 1.7.25)*
