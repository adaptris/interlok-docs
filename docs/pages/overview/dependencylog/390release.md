## Version 3.9.0 ##

### interlok-activemq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.9.9
- com.fasterxml.jackson.core:jackson-databind:2.9.9
- com.google.guava:guava:28.0-jre
- org.apache.qpid:proton-j:0.33.1
- org.springframework:spring-beans:4.3.24.RELEASE
- org.springframework:spring-context:4.3.24.RELEASE

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.9.9 *(from 2.9.8)*
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*
- com.google.guava:guava:28.0-jre *(from 27.1-jre)*
- org.apache.qpid:proton-j:0.33.1 *(from 0.32.0)*
- org.springframework:spring-beans:4.3.24.RELEASE *(from 4.3.23.RELEASE)*
- org.springframework:spring-context:4.3.24.RELEASE *(from 4.3.23.RELEASE)*

### interlok-amqp ###

#### New Dependencies ####
- com.rabbitmq:amqp-client:5.7.1
- org.apache.qpid:proton-j:0.33.1
- org.apache.qpid:qpid-client:6.3.4
- org.apache.qpid:qpid-jms-client:0.43.0

#### Updated Dependencies ####
- com.rabbitmq:amqp-client:5.7.1 *(from 5.6.0)*
- org.apache.qpid:proton-j:0.33.1 *(from 0.32.0)*
- org.apache.qpid:qpid-client:6.3.4 *(from 6.3.3)*
- org.apache.qpid:qpid-jms-client:0.43.0 *(from 0.40.0)*

### interlok-apache-http ###

#### New Dependencies ####
- org.apache.commons:commons-lang3:3.9
- org.apache.httpcomponents:httpclient:4.5.9

#### Updated Dependencies ####
- org.apache.commons:commons-lang3:3.9 *(from 3.8.1)*
- org.apache.httpcomponents:httpclient:4.5.9 *(from 4.5.8)*

### interlok-artemis ###

#### Initial Dependencies ####
- org.apache.activemq:artemis-jms-server:2.9.0

### interlok-aws-common ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.567

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-core:1.11.567 *(from 1.11.508)*

### interlok-aws-s3 ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.567

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-s3:1.11.567 *(from 1.11.508)*

### interlok-aws-sns ###

#### New Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.567

#### Updated Dependencies ####
- com.amazonaws:aws-java-sdk-sns:1.11.567 *(from 1.11.508)*

### interlok-aws-sqs ###

#### New Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.0.6
- com.amazonaws:aws-java-sdk-sqs:1.11.567
- com.fasterxml.jackson.core:jackson-databind:2.9.9
- org.apache.httpcomponents:httpclient:4.5.9

#### Updated Dependencies ####
- com.amazonaws:amazon-sqs-java-messaging-lib:1.0.6 *(from 1.0.5)*
- com.amazonaws:aws-java-sdk-sqs:1.11.567 *(from 1.11.508)*
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*
- org.apache.httpcomponents:httpclient:4.5.9 *(from 4.5.8)*

### interlok-cassandra ###

#### New Dependencies ####
- com.google.guava:guava:28.0-jre

#### Updated Dependencies ####
- com.google.guava:guava:28.0-jre *(from 27.1-jre)*

### interlok-common ###

#### New Dependencies ####
- org.apache.commons:commons-pool2:2.6.2
- org.eclipse.jetty.aggregate:jetty-all:9.4.19.v20190610

#### Updated Dependencies ####
- org.apache.commons:commons-pool2:2.6.2 *(from 2.6.1)*
- org.eclipse.jetty.aggregate:jetty-all:9.4.19.v20190610 *(from 9.4.15.v20190215)*

### interlok-core ###

#### New Dependencies ####
- io.github.classgraph:classgraph:4.8.37
- net.sf.saxon:Saxon-HE:9.9.1-3
- org.apache-extras.beanshell:bsh:2.0b6
- org.apache.activemq:artemis-jms-server:2.9.0
- org.apache.commons:commons-lang3:3.9
- org.apache.commons:commons-pool2:2.6.2
- org.bouncycastle:bcmail-jdk15on:1.62
- org.bouncycastle:bcpkix-jdk15on:1.62
- org.bouncycastle:bcprov-jdk15on:1.62
- org.eclipse.jetty.aggregate:jetty-all:9.4.19.v20190610
- org.jruby:jruby-complete:9.2.7.0

#### Updated Dependencies ####
- io.github.classgraph:classgraph:4.8.37 *(from 4.8.22)*
- net.sf.saxon:Saxon-HE:9.9.1-3 *(from 9.7.0-20)*
- org.apache.commons:commons-lang3:3.9 *(from 3.8.1)*
- org.apache.commons:commons-pool2:2.6.2 *(from 2.6.1)*
- org.bouncycastle:bcmail-jdk15on:1.62 *(from 1.61)*
- org.bouncycastle:bcpkix-jdk15on:1.62 *(from 1.61)*
- org.bouncycastle:bcprov-jdk15on:1.62 *(from 1.61)*
- org.eclipse.jetty.aggregate:jetty-all:9.4.19.v20190610 *(from 9.4.15.v20190215)*
- org.jruby:jruby-complete:9.2.7.0 *(from 9.2.6.0)*

#### Removed Dependencies ####
- ~~com.icegreen:greenmail:1.5.10~~

### interlok-csv ###

#### New Dependencies ####
- org.apache.commons:commons-csv:1.7

#### Updated Dependencies ####
- org.apache.commons:commons-csv:1.7 *(from 1.6)*

### interlok-csv-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*

### interlok-es-rest ###

#### New Dependencies ####
- joda-time:joda-time:2.10.2

#### Updated Dependencies ####
- joda-time:joda-time:2.10.2 *(from 2.10.1)*

### interlok-es5 ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*

### interlok-excel ###

#### New Dependencies ####
- org.apache.poi:poi-ooxml:4.1.0
- org.apache.poi:poi:4.1.0

#### Updated Dependencies ####
- org.apache.poi:poi-ooxml:4.1.0 *(from 4.0.1)*
- org.apache.poi:poi:4.1.0 *(from 4.0.1)*

### interlok-filesystem ###

#### New Dependencies ####
- org.apache.tika:tika-core:1.21

#### Updated Dependencies ####
- org.apache.tika:tika-core:1.21 *(from 1.20)*

### interlok-flyway ###

#### Initial Dependencies ####
- org.flywaydb:flyway-core:5.2.4

### interlok-gcloud-pubsub ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9
- com.google.cloud:google-cloud-pubsub:1.77.0
- com.google.guava:guava:28.0-jre
- org.apache.httpcomponents:httpclient:4.5.9

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*
- com.google.cloud:google-cloud-pubsub:1.77.0 *(from 1.67.0)*
- com.google.guava:guava:28.0-jre *(from 27.1-jre)*
- org.apache.httpcomponents:httpclient:4.5.9 *(from 4.5.8)*

### interlok-jclouds-blobstore ###

#### New Dependencies ####
- com.google.guava:guava:28.0-jre

#### Updated Dependencies ####
- com.google.guava:guava:28.0-jre *(from 27.1-jre)*

### interlok-jmx-jms ###

#### New Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:1.11.2
- com.rabbitmq:amqp-client:5.7.1
- com.solacesystems:sol-common:10.6.1
- com.solacesystems:sol-jcsmp:10.6.1
- com.solacesystems:sol-jms:10.6.1
- org.apache.activemq:activemq-client:5.15.9
- org.apache.qpid:proton-j:0.33.0
- org.apache.qpid:proton-jms:0.12.2
- org.apache.qpid:qpid-jms-client:0.42.0
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

#### Updated Dependencies ####
- com.rabbitmq.jms:rabbitmq-jms:1.11.2 *(from 1.6.0)*
- com.rabbitmq:amqp-client:5.7.1 *(from 4.0.2)*
- com.solacesystems:sol-common:10.6.1 *(from 10.1.1)*
- com.solacesystems:sol-jcsmp:10.6.1 *(from 10.1.1)*
- com.solacesystems:sol-jms:10.6.1 *(from 10.1.1)*
- org.apache.activemq:activemq-client:5.15.9 *(from 5.15.8)*
- org.apache.qpid:proton-j:0.33.0 *(from 0.17.0)*
- org.apache.qpid:proton-jms:0.12.2 *(from 0.12.1)*
- org.apache.qpid:qpid-jms-client:0.42.0 *(from 0.11.1)*
- org.slf4j:jcl-over-slf4j:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*
- org.slf4j:slf4j-log4j12:1.7.26 *(from 1.7.25)*

### interlok-jq ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9
- net.thisptr:jackson-jq:0.0.10

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*
- net.thisptr:jackson-jq:0.0.10 *(from 0.0.9)*

### interlok-jruby ###

#### New Dependencies ####
- org.jruby:jruby:9.2.7.0

#### Updated Dependencies ####
- org.jruby:jruby:9.2.7.0 *(from 9.2.6.0)*

### interlok-json ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.9.9
- com.fasterxml.jackson.core:jackson-databind:2.9.9
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.9.9
- com.flipkart.zjsonpatch:zjsonpatch:0.4.8
- com.google.guava:guava:28.0-jre

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-annotations:2.9.9 *(from 2.9.8)*
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*
- com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.9.9 *(from 2.9.8)*
- com.google.guava:guava:28.0-jre *(from 27.1-jre)*

### interlok-jsr107-cache ###

#### New Dependencies ####
- javax.cache:cache-api:1.1.1

#### Updated Dependencies ####
- javax.cache:cache-api:1.1.1 *(from 1.1.0)*

### interlok-kafka ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*

### interlok-kie ###

#### New Dependencies ####
- org.drools:drools-compiler:7.23.0.Final
- org.drools:drools-core:7.23.0.Final

#### Updated Dependencies ####
- org.drools:drools-compiler:7.23.0.Final *(from 7.20.0.Final)*
- org.drools:drools-core:7.23.0.Final *(from 7.20.0.Final)*

### interlok-licensing ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-licensing-demo ###

#### Initial Dependencies ####
- org.slf4j:slf4j-api:1.7.26

### interlok-mail ###

#### Initial Dependencies ####
- com.sun.mail:javax.mail:1.6.2

### interlok-mongodb ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9
- org.mongodb:mongodb-driver:3.10.2

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*
- org.mongodb:mongodb-driver:3.10.2 *(from 3.10.1)*

### interlok-monitor-agent ###

#### Initial Dependencies ####
- com.google.code.gson:gson:2.8.5
- org.apache.commons:commons-collections4:4.3
- org.slf4j:slf4j-api:1.7.26

### interlok-mqtt ###

#### New Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.9

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.9 *(from 4.5.8)*

### interlok-oauth-azure ###

#### New Dependencies ####
- com.microsoft.azure:adal4j:1.6.4

#### Updated Dependencies ####
- com.microsoft.azure:adal4j:1.6.4 *(from 1.6.3)*

### interlok-oauth-gcloud ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.9.9
- com.google.auth:google-auth-library-oauth2-http:0.16.1
- com.google.guava:guava:28.0-jre
- org.apache.httpcomponents:httpclient:4.5.9

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-core:2.9.9 *(from 2.9.8)*
- com.google.auth:google-auth-library-oauth2-http:0.16.1 *(from 0.15.0)*
- com.google.guava:guava:28.0-jre *(from 27.1-jre)*
- org.apache.httpcomponents:httpclient:4.5.9 *(from 4.5.8)*

### interlok-oauth-generic ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*

### interlok-oauth-salesforce ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9
- org.apache.httpcomponents:httpclient:4.5.9

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*
- org.apache.httpcomponents:httpclient:4.5.9 *(from 4.5.8)*

### interlok-okhttp ###

#### New Dependencies ####
- com.squareup.okhttp3:okhttp:3.14.2

#### Updated Dependencies ####
- com.squareup.okhttp3:okhttp:3.14.2 *(from 3.14.0)*

### interlok-pdf ###

#### New Dependencies ####
- com.google.guava:guava:28.0-jre
- net.sf.cssbox:pdf2dom:1.8
- org.apache.pdfbox:fontbox:2.0.15
- org.apache.pdfbox:pdfbox-tools:2.0.15
- org.apache.pdfbox:pdfbox:2.0.15
- xerces:xercesImpl:2.12.0

#### Updated Dependencies ####
- org.apache.pdfbox:fontbox:2.0.15 *(from 2.0.14)*

### interlok-profiler ###

#### New Dependencies ####
- org.aspectj:aspectjrt:1.9.4
- org.aspectj:aspectjtools:1.9.4
- org.aspectj:aspectjweaver:1.9.4

#### Updated Dependencies ####
- org.aspectj:aspectjrt:1.9.4 *(from 1.9.2)*
- org.aspectj:aspectjtools:1.9.4 *(from 1.9.2)*
- org.aspectj:aspectjweaver:1.9.4 *(from 1.9.2)*

### interlok-profiler-metric-services ###

#### Initial Dependencies ####
- org.codehaus.groovy:groovy-json:2.5.7
- org.codehaus.groovy:groovy:2.5.7

### interlok-schema ###

#### New Dependencies ####
- xerces:xercesImpl:2.12.0

### interlok-service-tester ###

#### New Dependencies ####
- com.github.tomakehurst:wiremock:2.23.2
- org.apache.ant:ant-junit:1.10.6

#### Updated Dependencies ####
- com.github.tomakehurst:wiremock:2.23.2 *(from 2.22.0)*
- org.apache.ant:ant-junit:1.10.6 *(from 1.10.5)*

### interlok-shell ###

#### New Dependencies ####
- org.bouncycastle:bcpkix-jdk15on:1.62
- org.bouncycastle:bcprov-jdk15on:1.62
- org.codehaus.groovy:groovy-all:2.5.7

#### Updated Dependencies ####
- org.bouncycastle:bcpkix-jdk15on:1.62 *(from 1.61)*
- org.bouncycastle:bcprov-jdk15on:1.62 *(from 1.61)*
- org.codehaus.groovy:groovy-all:2.5.7 *(from 2.5.2)*

### interlok-solace ###

#### New Dependencies ####
- com.solacesystems:sol-common:10.6.0
- com.solacesystems:sol-jcsmp:10.6.0
- com.solacesystems:sol-jms:10.6.0
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- com.solacesystems:sol-common:10.6.0 *(from 7.2.1.148)*
- com.solacesystems:sol-jcsmp:10.6.0 *(from 7.2.1.148)*
- com.solacesystems:sol-jms:10.6.0 *(from 7.2.1.148)*
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*

### interlok-stubs ###

#### New Dependencies ####
- io.github.classgraph:classgraph:4.8.37
- net.sf.saxon:Saxon-HE:9.9.1-3
- org.apache-extras.beanshell:bsh:2.0b6
- org.apache.activemq:artemis-jms-server:2.9.0
- org.apache.commons:commons-lang3:3.9
- org.apache.commons:commons-pool2:2.6.2
- org.bouncycastle:bcmail-jdk15on:1.62
- org.bouncycastle:bcpkix-jdk15on:1.62
- org.bouncycastle:bcprov-jdk15on:1.62
- org.eclipse.jetty.aggregate:jetty-all:9.4.19.v20190610
- org.jruby:jruby-complete:9.2.7.0

#### Updated Dependencies ####
- io.github.classgraph:classgraph:4.8.37 *(from 4.8.22)*
- net.sf.saxon:Saxon-HE:9.9.1-3 *(from 9.7.0-20)*
- org.apache.commons:commons-lang3:3.9 *(from 3.8.1)*
- org.apache.commons:commons-pool2:2.6.2 *(from 2.6.1)*
- org.bouncycastle:bcmail-jdk15on:1.62 *(from 1.61)*
- org.bouncycastle:bcpkix-jdk15on:1.62 *(from 1.61)*
- org.bouncycastle:bcprov-jdk15on:1.62 *(from 1.61)*
- org.eclipse.jetty.aggregate:jetty-all:9.4.19.v20190610 *(from 9.4.15.v20190215)*
- org.jruby:jruby-complete:9.2.7.0 *(from 9.2.6.0)*

#### Removed Dependencies ####
- ~~com.icegreen:greenmail:1.5.10~~

### interlok-vcs-git ###

#### New Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.9
- org.eclipse.jgit:org.eclipse.jgit:5.4.0.201906121030-r

#### Updated Dependencies ####
- org.apache.httpcomponents:httpclient:4.5.9 *(from 4.5.8)*
- org.eclipse.jgit:org.eclipse.jgit:5.4.0.201906121030-r *(from 5.3.0.201903130848-r)*

### interlok-vertx ###

#### New Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9

#### Updated Dependencies ####
- com.fasterxml.jackson.core:jackson-databind:2.9.9 *(from 2.9.8)*

### interlok-xa-activemq ###

#### Initial Dependencies ####
- javax.transaction:jta:1.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

### interlok-xa-atomikos ###

#### Initial Dependencies ####
- com.atomikos:transactions-jms:3.8.0
- javax.transaction:jta:1.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

### interlok-xa-jms ###

#### Initial Dependencies ####
- javax.transaction:jta:1.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

### interlok-xa-solace ###

#### Initial Dependencies ####
- com.solacesystems:sol-common:10.6.0
- com.solacesystems:sol-jcsmp:10.6.0
- com.solacesystems:sol-jms:10.6.0
- javax.transaction:jta:1.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

### interlok-xa-tibco ###

#### Initial Dependencies ####
- com.tibco:tibjms:6.3.0
- com.tibco:tibrv:7.5.1
- javax.transaction:jta:1.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

### interlok-xa-wmq ###

#### Initial Dependencies ####
- com.ibm:mq:6.0.0.0
- com.ibm:mqjms:6.0.0.0
- javax.transaction:jta:1.1
- org.slf4j:jcl-over-slf4j:1.7.26
- org.slf4j:slf4j-api:1.7.26
- org.slf4j:slf4j-log4j12:1.7.26

### interlok-xml-security ###

#### New Dependencies ####
- org.slf4j:slf4j-api:1.7.26

#### Updated Dependencies ####
- org.slf4j:slf4j-api:1.7.26 *(from 1.7.25)*
