## Version 4.8.0 ##

### bip-services ###
| Initial Dependencies |
| -------- |
| net.minidev:json-smart:2.4.10 |
| org.slf4j:slf4j-api:1.7.35 |

### interlok-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.0)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.qpid:proton-j:0.34.1 *(from 0.34.0)* |  |
|  | org.springframework:spring-beans:5.3.27 *(from 5.3.23)* |  |
|  | org.springframework:spring-context:5.3.27 *(from 5.3.23)* |  |

### interlok-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.17.0 *(from 5.16.0)* |  |
|  | org.apache.qpid:proton-j:0.34.1 *(from 0.34.0)* |  |
|  | org.apache.qpid:qpid-jms-client:2.2.0 *(from 2.1.0)* |  |

### interlok-apache-geode ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-core: | org.apache.shiro:shiro-core:1.11.0 *(from 1.10.0)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.springframework:spring-web:5.3.26 *(from 5.3.23)* |  |

### interlok-apache-http ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents:httpclient:4.5.14 *(from 4.5.13)* |  |

### interlok-apache-http-async ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents:httpclient:4.5.14 *(from 4.5.13)* |  |

### interlok-artemis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.activemq:artemis-jms-server:2.28.0 *(from 2.26.0)* |  |
|  | org.apache.activemq:artemis-server:2.28.0 *(from 2.26.0)* |  |
|  | org.apache.commons:commons-configuration2:2.9.0 *(from 2.8.0)* |  |

### interlok-aws-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.447 *(from 1.12.319)* |  |
| com.amazonaws:aws-java-sdk-sts: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kinesis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:amazon-kinesis-client:1.14.10 *(from 1.14.8)* |  |
| com.amazonaws:aws-java-sdk-kinesis: | com.amazonaws:amazon-kinesis-producer:0.15.5 *(from 0.14.12)* |  |
| com.charleskorn.kaml:kaml:0.53.0 | com.amazonaws:aws-java-sdk-bom:1.12.447 *(from 1.12.319)* |  |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.google.protobuf:protobuf-java:3.22.3 *(from 3.21.7)* |  |
| com.fasterxml.jackson.core:jackson-databind: | io.netty:netty-bom:4.1.91.Final *(from 4.1.87.Final)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.apache.commons:commons-compress:1.23.0 *(from 1.21)* |  |
| io.netty:netty-buffer: | org.apache.kafka:kafka-clients:3.4.0 *(from 2.8.2)* |  |
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
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.447 *(from 1.12.319)* |  |
| com.amazonaws:aws-java-sdk-kinesis: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.447 *(from 1.12.319)* |  |
| com.amazonaws:aws-java-sdk-kms: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-s3 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.447 *(from 1.12.319)* |  |
| com.amazonaws:aws-java-sdk-s3: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sns ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.447 *(from 1.12.319)* |  |
| com.amazonaws:aws-java-sdk-sns: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sqs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:aws-java-sdk-core:1.12.447 *(from 1.12.319)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-sqs:1.12.447 *(from 1.12.319)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-azure-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.microsoft.azure:msal4j:1.13.7 *(from 1.13.2)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-xml: | io.netty:netty-codec-http2:4.1.91.Final *(from 4.1.87.Final)* |  |
| com.fasterxml.jackson.datatype:jackson-datatype-jsr310: | io.netty:netty-codec-http:4.1.91.Final *(from 4.1.87.Final)* |  |
|  | io.netty:netty-codec:4.1.91.Final *(from 4.1.87.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.91.Final *(from 4.1.87.Final)* |  |
|  | io.netty:netty-handler:4.1.91.Final *(from 4.1.87.Final)* |  |
|  | io.netty:netty-resolver-dns:4.1.91.Final *(from 4.1.87.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.91.Final *(from 4.1.87.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.91.Final *(from 4.1.87.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.91.Final *(from 4.1.87.Final)* |  |

### interlok-azure-cosmosdb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.microsoft.azure:azure-documentdb:2.6.5 *(from 2.6.4)* |  |

### interlok-cassandra ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.logging.log4j:log4j-1.2-api:2.20.0 *(from 2.19.0)* |  |
|  | org.apache.logging.log4j:log4j-api:2.20.0 *(from 2.19.0)* |  |
|  | org.apache.logging.log4j:log4j-core:2.20.0 *(from 2.19.0)* |  |
|  | org.apache.logging.log4j:log4j-slf4j2-impl:2.20.0 *(from 2.19.0)* |  |

### interlok-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.glassfish:jakarta.el:3.0.4 | com.github.mwiede:jsch:0.2.8 *(from 0.2.5)* | ~~org.glassfish:javax.el:3.0.1-b12~~ |
|  | org.apache.activemq:activemq-client:5.17.3 *(from 5.17.2)* |  |
|  | org.codehaus.jettison:jettison:1.5.4 *(from 1.5.3)* |  |

### interlok-csv-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |

### interlok-elastic-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | com.jayway.jsonpath:json-path:2.8.0 *(from 2.7.0)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-elastic-rest ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | com.jayway.jsonpath:json-path:2.8.0 *(from 2.7.0)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-elastic-sdk ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | com.jayway.jsonpath:json-path:2.8.0 *(from 2.7.0)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-filesystem ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.commons:commons-compress:1.23.0 *(from 1.21)* |  |
|  | org.json:json:20230227 *(from 20220924)* |  |

### interlok-gcloud-pubsub ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
|  | com.google.cloud:google-cloud-pubsub:1.123.8 *(from 1.121.1)* |  |
|  | org.apache.httpcomponents:httpclient:4.5.14 *(from 4.5.13)* |  |

### interlok-jmx-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.activemq:activemq-client:5.17.4 *(from 5.17.2)* |  |
|  | org.springframework:spring-aop:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-beans:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-context:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-core:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-jms:5.3.26 *(from 5.3.23)* |  |

### interlok-jmx-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.qpid:proton-j:0.34.1 *(from 0.34.0)* |  |
|  | org.springframework:spring-aop:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-beans:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-context:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-core:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-jms:5.3.26 *(from 5.3.23)* |  |

### interlok-jmx-jms-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.springframework:spring-aop:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-beans:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-context:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-core:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-jms:5.3.26 *(from 5.3.23)* |  |

### interlok-jmx-jms-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.activemq:activemq-amqp:5.17.4 *(from 5.17.2)* |  |
|  | org.apache.activemq:activemq-broker:5.17.4 *(from 5.17.2)* |  |
|  | org.apache.activemq:activemq-jaas:5.17.4 *(from 5.17.2)* |  |
|  | org.apache.activemq:activemq-kahadb-store:5.17.4 *(from 5.17.2)* |  |
|  | org.springframework:spring-aop:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-beans:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-context:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-core:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-jms:5.3.26 *(from 5.3.23)* |  |

### interlok-jmx-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.springframework:spring-aop:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-beans:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-context:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-core:5.3.26 *(from 5.3.23)* |  |
|  | org.springframework:spring-jms:5.3.26 *(from 5.3.23)* |  |

### interlok-jolokia ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jolokia:jolokia-core:1.7.2 *(from 1.7.1)* |  |
|  | org.jolokia:jolokia-jsr160:1.7.2 *(from 1.7.1)* |  |

### interlok-jq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
|  | net.thisptr:jackson-jq-extra:1.0.0-preview.20230409 *(from 1.0.0-preview.20220705)* |  |
|  | net.thisptr:jackson-jq:1.0.0-preview.20230409 *(from 1.0.0-preview.20220705)* |  |

### interlok-jruby ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jruby:jruby:9.4.2.0 *(from 9.4.0.0)* |  |

### interlok-jslt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
|  | com.schibsted.spt.data:jslt:0.1.14 *(from 0.1.13)* |  |

### interlok-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.flipkart.zjsonpatch:zjsonpatch:0.4.14 *(from 0.4.12)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.github.erosb:everit-json-schema:1.14.2 *(from 1.14.1)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: | com.jayway.jsonpath:json-path:2.8.0 *(from 2.7.0)* |  |
| net.minidev:json-smart:2.4.10 | org.json:json:20230227 *(from 20220924)* |  |

### interlok-json-streaming ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.github.jsurfer:jsurfer-core:1.6.4 *(from 1.6.3)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.github.jsurfer:jsurfer-gson:1.6.4 *(from 1.6.3)* |  |
|  | com.github.jsurfer:jsurfer-jackson:1.6.4 *(from 1.6.3)* |  |
|  | com.github.jsurfer:jsurfer-jsonsimple:1.6.4 *(from 1.6.3)* |  |

### interlok-json-web-token ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
|  | org.json:json:20230227 *(from 20220924)* |  |

### interlok-kafka ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* | ~~org.apache.kafka:kafka_2.11:2.4.1~~ |
| org.apache.kafka:kafka_2.13:3.4.0 | org.apache.kafka:kafka-clients:3.4.0 *(from 2.4.1)* |  |
|  | org.apache.zookeeper:zookeeper:3.8.1 *(from 3.8.0)* |  |

### interlok-logging ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.logging.log4j:log4j-api:2.20.0 *(from 2.19.0)* |  |
|  | org.apache.logging.log4j:log4j-core:2.20.0 *(from 2.19.0)* |  |

### interlok-mongodb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
|  | org.mongodb:mongodb-driver:3.12.13 *(from 3.12.11)* |  |

### interlok-mqtt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents:httpclient:4.5.14 *(from 4.5.13)* |  |

### interlok-nats ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.nats:jnats:2.16.10 *(from 2.16.1)* |  |

### interlok-oauth-azure ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | net.minidev:json-smart:2.4.10 *(from 2.4.8)* |  |

### interlok-oauth-gcloud ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents:httpclient:4.5.14 *(from 4.5.13)* |  |

### interlok-oauth-generic ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
|  | com.jayway.jsonpath:json-path:2.8.0 *(from 2.7.0)* |  |

### interlok-oauth-salesforce ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
|  | org.apache.httpcomponents:httpclient:4.5.14 *(from 4.5.13)* |  |

### interlok-pdf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.xmlgraphics:fop:2.8 *(from 2.7)* |  |

### interlok-profiler ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.aspectj:aspectjrt:1.9.19 *(from 1.9.9.1)* |  |
|  | org.aspectj:aspectjtools:1.9.19 *(from 1.9.9.1)* |  |
|  | org.aspectj:aspectjweaver:1.9.19 *(from 1.9.9.1)* |  |

### interlok-rabbitmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.17.0 *(from 5.16.0)* |  |

### interlok-rest-metrics-jvm ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-core:1.10.6 *(from 1.9.5)* |  |

### interlok-rest-provider-datadog ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-registry-datadog:1.10.6 *(from 1.9.5)* |  |

### interlok-rest-provider-prometheus ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-registry-prometheus:1.10.6 *(from 1.9.5)* |  |

### interlok-service-tester-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.jayway.jsonpath:json-path:2.8.0 *(from 2.7.0)* |  |
|  | org.json:json:20230227 *(from 20220924)* |  |

### interlok-service-tester-wiremock ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.2 *(from 2.14.1)* |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.jayway.jsonpath:json-path:2.8.0 |  |  |
| commons-fileupload:commons-fileupload:1.5 |  |  |

### interlok-swift ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.prowidesoftware:pw-swift-core:SRU2022-9.3.14 *(from SRU2021-9.2.18)* |  |

### interlok-vcs-git ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents:httpclient:4.5.14 *(from 4.5.13)* |  |

### interlok-webservice-cxf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.glassfish.jaxb:jaxb-runtime:2.3.8 *(from 2.3.2)* |  |

### interlok-webspheremq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.3.2.0 *(from 9.3.0.1)* |  |
