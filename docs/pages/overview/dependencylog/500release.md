## Version 5.0.0 ##

### interlok-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | org.apache.activemq:activemq-amqp:5.18.3 *(from 5.18.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.activemq:activemq-broker:5.18.3 *(from 5.18.2)* |  |
|  | org.apache.activemq:activemq-client:5.18.3 *(from 5.18.2)* |  |
|  | org.apache.activemq:activemq-jaas:5.18.3 *(from 5.18.2)* |  |
|  | org.apache.activemq:activemq-kahadb-store:5.18.3 *(from 5.18.2)* |  |
|  | org.apache.activemq:activemq-mqtt:5.18.3 *(from 5.18.2)* |  |
|  | org.apache.activemq:activemq-spring:5.18.3 *(from 5.18.2)* |  |
|  | org.apache.activemq:activemq-stomp:5.18.3 *(from 5.18.2)* |  |

### interlok-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.20.0 *(from 5.19.0)* | ~~javax.jms:javax.jms-api:2.0.1~~ |

### interlok-apache-geode ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-artemis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.activemq:artemis-jms-server:2.31.2 *(from 2.31.0)* |  |
|  | org.apache.activemq:artemis-server:2.31.2 *(from 2.31.0)* |  |

### interlok-aws-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.576 *(from 1.12.567)* |  |
| com.amazonaws:aws-java-sdk-sts: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kinesis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.576 *(from 1.12.567)* |  |
| com.amazonaws:aws-java-sdk-kinesis: | com.google.protobuf:protobuf-java:3.25.0 *(from 3.24.4)* |  |
| com.fasterxml.jackson.core:jackson-annotations: | com.squareup.okio:okio-fakefilesystem:3.6.0 *(from 3.5.0)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.squareup.okio:okio:3.6.0 *(from 3.5.0)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |
| io.netty:netty-buffer: |  |  |
| io.netty:netty-codec-http: |  |  |
| io.netty:netty-codec: |  |  |
| io.netty:netty-common: |  |  |
| io.netty:netty-handler: |  |  |
| io.netty:netty-transport-native-epoll: |  |  |
| io.netty:netty-transport-native-kqueue: |  |  |
| io.netty:netty-transport-native-unix-common: |  |  |
| io.netty:netty-transport: |  |  |

### interlok-aws-kinesis-sdk ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.576 *(from 1.12.567)* |  |
| com.amazonaws:aws-java-sdk-kinesis: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.576 *(from 1.12.567)* |  |
| com.amazonaws:aws-java-sdk-kms: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-s3 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.576 *(from 1.12.567)* |  |
| com.amazonaws:aws-java-sdk-s3: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sns ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.576 *(from 1.12.567)* |  |
| com.amazonaws:aws-java-sdk-sns: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sqs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:aws-java-sdk-core:1.12.576 *(from 1.12.567)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-sqs:1.12.576 *(from 1.12.567)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws2-common ###
| Initial Dependencies |
| -------- |
| com.fasterxml.jackson.core:jackson-annotations:2.15.3 |
| com.fasterxml.jackson.core:jackson-core:2.15.3 |
| com.fasterxml.jackson.core:jackson-databind:2.15.3 |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.15.3 |
| org.slf4j:jcl-over-slf4j:2.0.9 |
| org.slf4j:slf4j-api:2.0.9 |
| software.amazon.awssdk:apache-client:2.21.15 |
| software.amazon.awssdk:sdk-core:2.21.15 |
| software.amazon.awssdk:sts:2.21.15 |

### interlok-aws2-kms ###
| Initial Dependencies |
| -------- |
| com.fasterxml.jackson.core:jackson-annotations:2.15.3 |
| com.fasterxml.jackson.core:jackson-core:2.15.3 |
| com.fasterxml.jackson.core:jackson-databind:2.15.3 |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.15.3 |
| org.slf4j:jcl-over-slf4j:2.0.9 |
| org.slf4j:slf4j-api:2.0.9 |
| software.amazon.awssdk:kms:2.21.15 |
| software.amazon.awssdk:sdk-core:2.21.15 |

### interlok-aws2-s3 ###
| Initial Dependencies |
| -------- |
| com.fasterxml.jackson.core:jackson-annotations:2.15.3 |
| com.fasterxml.jackson.core:jackson-core:2.15.3 |
| com.fasterxml.jackson.core:jackson-databind:2.15.3 |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.15.3 |
| org.slf4j:jcl-over-slf4j:2.0.9 |
| org.slf4j:slf4j-api:2.0.9 |
| software.amazon.awssdk:s3:2.21.15 |
| software.amazon.awssdk:sdk-core:2.21.15 |

### interlok-azure-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.azure:azure-identity:1.10.4 *(from 1.10.3)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.azure:azure-storage-file-datalake:12.17.1 *(from 12.17.0)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-xml: | com.microsoft.azure:msal4j:1.14.0 *(from 1.13.10)* |  |
| com.fasterxml.jackson.datatype:jackson-datatype-jsr310: | com.microsoft.graph:microsoft-graph:5.75.0 *(from 5.74.0)* |  |
|  | com.squareup.okhttp3:okhttp:4.12.0 *(from 4.11.0)* |  |

### interlok-azure-cosmosdb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-cassandra ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.datastax.oss:java-driver-core:4.17.0 |  | ~~com.datastax.cassandra:cassandra-driver-core:3.11.5~~ |
| com.datastax.oss:java-driver-mapper-runtime:4.17.0 |  | ~~com.datastax.cassandra:cassandra-driver-mapping:3.11.5~~ |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.eclipse.jetty.http2:http2-client:10.0.18 | commons-io:commons-io:2.15.0 *(from 2.14.0)* | ~~org.eclipse.jetty.aggregate:jetty-all:9.4.53.v20231009~~ |
| org.eclipse.jetty.http2:http2-common:10.0.18 | org.apache.logging.log4j:log4j-1.2-api:2.21.1 *(from 2.20.0)* |  |
| org.eclipse.jetty.http2:http2-hpack:10.0.18 | org.apache.logging.log4j:log4j-api:2.21.1 *(from 2.20.0)* |  |
| org.eclipse.jetty.http2:http2-server:10.0.18 | org.apache.logging.log4j:log4j-core:2.21.1 *(from 2.20.0)* |  |
| org.eclipse.jetty.websocket:websocket-javax-client:10.0.18 | org.apache.logging.log4j:log4j-slf4j2-impl:2.21.1 *(from 2.20.0)* |  |
| org.eclipse.jetty.websocket:websocket-javax-server:10.0.18 |  |  |
| org.eclipse.jetty:jetty-alpn-client:10.0.18 |  |  |
| org.eclipse.jetty:jetty-alpn-java-client:10.0.18 |  |  |
| org.eclipse.jetty:jetty-alpn-java-server:10.0.18 |  |  |
| org.eclipse.jetty:jetty-alpn-server:10.0.18 |  |  |
| org.eclipse.jetty:jetty-annotations:10.0.18 |  |  |
| org.eclipse.jetty:jetty-client:10.0.18 |  |  |
| org.eclipse.jetty:jetty-deploy:10.0.18 |  |  |
| org.eclipse.jetty:jetty-http:10.0.18 |  |  |
| org.eclipse.jetty:jetty-io:10.0.18 |  |  |
| org.eclipse.jetty:jetty-jaspi:10.0.18 |  |  |
| org.eclipse.jetty:jetty-jmx:10.0.18 |  |  |
| org.eclipse.jetty:jetty-jndi:10.0.18 |  |  |
| org.eclipse.jetty:jetty-plus:10.0.18 |  |  |
| org.eclipse.jetty:jetty-quickstart:10.0.18 |  |  |
| org.eclipse.jetty:jetty-rewrite:10.0.18 |  |  |
| org.eclipse.jetty:jetty-security:10.0.18 |  |  |
| org.eclipse.jetty:jetty-server:10.0.18 |  |  |
| org.eclipse.jetty:jetty-servlet:10.0.18 |  |  |
| org.eclipse.jetty:jetty-servlets:10.0.18 |  |  |
| org.eclipse.jetty:jetty-util-ajax:10.0.18 |  |  |
| org.eclipse.jetty:jetty-util:10.0.18 |  |  |
| org.eclipse.jetty:jetty-webapp:10.0.18 |  |  |
| org.eclipse.jetty:jetty-xml:10.0.18 |  |  |

### interlok-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.eclipse.jetty.http2:http2-client:10.0.18 | com.github.mwiede:jsch:0.2.12 *(from 0.2.11)* | ~~org.eclipse.jetty.aggregate:jetty-all:9.4.53.v20231009~~ |
| org.eclipse.jetty.http2:http2-common:10.0.18 | com.zaxxer:HikariCP:5.1.0 *(from 5.0.1)* |  |
| org.eclipse.jetty.http2:http2-hpack:10.0.18 | commons-io:commons-io:2.15.0 *(from 2.14.0)* |  |
| org.eclipse.jetty.http2:http2-server:10.0.18 | org.apache.activemq:activemq-client:5.18.3 *(from 5.18.2)* |  |
| org.eclipse.jetty.websocket:websocket-javax-client:10.0.18 | org.apache.commons:commons-text:1.11.0 *(from 1.10.0)* |  |
| org.eclipse.jetty.websocket:websocket-javax-server:10.0.18 |  |  |
| org.eclipse.jetty:jetty-alpn-client:10.0.18 |  |  |
| org.eclipse.jetty:jetty-alpn-java-client:10.0.18 |  |  |
| org.eclipse.jetty:jetty-alpn-java-server:10.0.18 |  |  |
| org.eclipse.jetty:jetty-alpn-server:10.0.18 |  |  |
| org.eclipse.jetty:jetty-annotations:10.0.18 |  |  |
| org.eclipse.jetty:jetty-client:10.0.18 |  |  |
| org.eclipse.jetty:jetty-deploy:10.0.18 |  |  |
| org.eclipse.jetty:jetty-http:10.0.18 |  |  |
| org.eclipse.jetty:jetty-io:10.0.18 |  |  |
| org.eclipse.jetty:jetty-jaspi:10.0.18 |  |  |
| org.eclipse.jetty:jetty-jmx:10.0.18 |  |  |
| org.eclipse.jetty:jetty-jndi:10.0.18 |  |  |
| org.eclipse.jetty:jetty-plus:10.0.18 |  |  |
| org.eclipse.jetty:jetty-quickstart:10.0.18 |  |  |
| org.eclipse.jetty:jetty-rewrite:10.0.18 |  |  |
| org.eclipse.jetty:jetty-security:10.0.18 |  |  |
| org.eclipse.jetty:jetty-server:10.0.18 |  |  |
| org.eclipse.jetty:jetty-servlet:10.0.18 |  |  |
| org.eclipse.jetty:jetty-servlets:10.0.18 |  |  |
| org.eclipse.jetty:jetty-util-ajax:10.0.18 |  |  |
| org.eclipse.jetty:jetty-util:10.0.18 |  |  |
| org.eclipse.jetty:jetty-webapp:10.0.18 |  |  |
| org.eclipse.jetty:jetty-xml:10.0.18 |  |  |
| org.flywaydb:flyway-core:8.5.13 |  |  |

### interlok-csv-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-elastic-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.logging.log4j:log4j-api:2.21.1 *(from 2.20.0)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-elastic-rest ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.logging.log4j:log4j-api:2.21.1 *(from 2.20.0)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-elastic-sdk ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.logging.log4j:log4j-api:2.21.1 *(from 2.20.0)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-filesystem ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.tika:tika-core:2.9.1 *(from 2.9.0)* |  |

### interlok-gcloud-pubsub ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.google.cloud:google-cloud-pubsub:1.125.9 *(from 1.125.6)* |  |
|  | io.grpc:grpc-alts:1.59.0 *(from 1.58.0)* |  |
|  | io.grpc:grpc-auth:1.59.0 *(from 1.58.0)* |  |
|  | io.grpc:grpc-context:1.59.0 *(from 1.58.0)* |  |
|  | io.grpc:grpc-googleapis:1.59.0 *(from 1.58.0)* |  |
|  | io.grpc:grpc-inprocess:1.59.0 *(from 1.58.0)* |  |
|  | io.grpc:grpc-netty:1.59.0 *(from 1.58.0)* |  |
|  | io.grpc:grpc-protobuf:1.59.0 *(from 1.58.0)* |  |
|  | io.grpc:grpc-services:1.59.0 *(from 1.58.0)* |  |
|  | io.grpc:grpc-stub:1.59.0 *(from 1.58.0)* |  |

### interlok-jms3-common ###
| Initial Dependencies |
| -------- |
| io.netty:netty-bom:4.1.100.Final |
| jakarta.jms:jakarta.jms-api:3.1.0 |
| org.apache.activemq:artemis-jakarta-client:2.31.2 |
| org.apache.geronimo.specs:geronimo-jms_2.0_spec:1.0-alpha-2 |
| org.slf4j:jcl-over-slf4j:2.0.9 |
| org.slf4j:slf4j-api:2.0.9 |

### interlok-jmx-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | commons-io:commons-io:2.15.0 *(from 2.14.0)* |  |

### interlok-jmx-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | commons-io:commons-io:2.15.0 *(from 2.14.0)* |  |

### interlok-jmx-jms-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | commons-io:commons-io:2.15.0 *(from 2.14.0)* |  |

### interlok-jmx-jms-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | commons-io:commons-io:2.15.0 *(from 2.14.0)* | ~~junit:junit:4.13.2~~ |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| org.junit.jupiter:junit-jupiter-engine:5.10.0 |  |  |

### interlok-jmx-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | commons-io:commons-io:2.15.0 *(from 2.14.0)* |  |

### interlok-jolokia ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.eclipse.jetty:jetty-bom:10.0.18 |  | ~~org.eclipse.jetty.aggregate:jetty-all:9.4.53.v20231009~~ |

### interlok-jq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:2.0.9 *(from 2.0.7)* |  |

### interlok-jruby ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jruby:jruby:9.4.4.0 *(from 9.4.3.0)* |  |

### interlok-jslt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:2.0.9 *(from 2.0.7)* |  |

### interlok-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.github.erosb:everit-json-schema:1.14.3 *(from 1.14.2)* |  |
| com.fasterxml.jackson.core:jackson-core: | org.slf4j:slf4j-api:2.0.9 *(from 2.0.7)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-json-streaming ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | org.slf4j:slf4j-api:2.0.9 *(from 2.0.7)* |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-json-web-token ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:2.0.9 *(from 2.0.7)* |  |

### interlok-kafka ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-logging ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.logging.log4j:log4j-api:2.21.1 *(from 2.20.0)* |  |
|  | org.apache.logging.log4j:log4j-core:2.21.1 *(from 2.20.0)* |  |

### interlok-mongodb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-nats ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.nats:jnats:2.17.1 *(from 2.17.0)* |  |

### interlok-oauth-azure ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.nimbusds:nimbus-jose-jwt:9.37 *(from 9.36)* |  |

### interlok-oauth-gcloud ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.grpc:grpc-context:1.59.0 *(from 1.58.0)* |  |

### interlok-oauth-generic ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-oauth-salesforce ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-okhttp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.squareup.okhttp3:okhttp:4.12.0 *(from 4.11.0)* |  |

### interlok-pdf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | commons-io:commons-io:2.15.0 *(from 2.14.0)* |  |

### interlok-rabbitmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.20.0 *(from 5.19.0)* | ~~javax.jms:javax.jms-api:2.0.1~~ |

### interlok-scripting ###
| Initial Dependencies |
| -------- |
| org.graalvm.js:js-scriptengine:23.0.2 |
| org.graalvm.js:js:23.0.2 |
| org.graalvm.sdk:graal-sdk:23.0.2 |
| org.slf4j:slf4j-api:2.0.9 |

### interlok-service-tester ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | commons-io:commons-io:2.15.0 *(from 2.14.0)* |  |

### interlok-service-tester-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-service-tester-wiremock ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | org.eclipse.jetty:jetty-bom:10.0.18 *(from 9.4.53.v20231009)* | ~~com.github.tomakehurst:wiremock-jre8:2.35.1~~ |
| com.fasterxml.jackson.core:jackson-core: |  | ~~org.json:json:20231013~~ |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| io.netty:netty-bom:4.1.100.Final |  |  |
| io.swagger.parser.v3:swagger-parser:2.1.18 |  |  |
| org.mock-server:mockserver-netty:5.15.0 |  |  |
| org.mozilla:rhino:1.7.14 |  |  |
| org.yaml:snakeyaml:2.2 |  |  |

### interlok-sshtunnel ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.12 *(from 0.2.11)* |  |

### interlok-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.junit.jupiter:junit-jupiter-api:5.10.1 |  | ~~junit:junit:4.13.2~~ |
| org.junit.jupiter:junit-jupiter-engine:5.10.1 |  |  |

### interlok-vcs-git ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.12 *(from 0.2.11)* |  |
|  | org.eclipse.jgit:org.eclipse.jgit.ssh.jsch:6.7.0.202309050840-r *(from 5.13.2.202306221912-r)* |  |
|  | org.eclipse.jgit:org.eclipse.jgit:6.7.0.202309050840-r *(from 5.13.2.202306221912-r)* |  |

### interlok-webspheremq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.3.4.0 *(from 9.3.3.1)* |  |

### interlok-xa-wmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.3.4.0 *(from 9.3.3.1)* |  |
