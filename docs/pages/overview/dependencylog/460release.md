## Version 4.6.0 ##

### interlok-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.activemq:activemq-amqp:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-broker:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-client:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-jaas:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-kahadb-store:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-mqtt:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-spring:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-stomp:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.qpid:proton-j:0.34.0 *(from 0.33.10)* |  |
|  | org.springframework:spring-beans:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-context:5.3.23 *(from 5.3.20)* |  |

### interlok-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.16.0 *(from 5.14.2)* |  |
|  | io.netty:netty-buffer:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec-http:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-common:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-handler:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | org.apache.qpid:proton-j:0.34.0 *(from 0.33.10)* |  |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-apache-geode ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.core:jackson-core: | org.apache.geode:geode-core:1.15.1 *(from 1.14.4)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.shiro:shiro-core:1.10.0 *(from 1.9.0)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
|  | org.springframework:spring-web:5.3.23 *(from 5.3.20)* |  |

### interlok-apache-http ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-apache-http-async ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-apache-http5 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-artemis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.netty:netty-buffer:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec-http:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-common:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-handler:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | org.apache.activemq:artemis-jms-server:2.26.0 *(from 2.22.0)* |  |
|  | org.apache.activemq:artemis-server:2.26.0 *(from 2.22.0)* |  |
|  | org.apache.commons:commons-configuration2:2.8.0 *(from 2.7)* |  |

### interlok-as400 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-aws-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-bom:1.12.319 | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* | ~~com.amazonaws:aws-java-sdk-core:1.12.228~~ |
| com.amazonaws:aws-java-sdk-core: | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* | ~~com.amazonaws:aws-java-sdk-sts:1.12.228~~ |
| com.amazonaws:aws-java-sdk-sts: | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kinesis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-bom:1.12.319 | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* | ~~com.amazonaws:aws-java-sdk-core:1.12.228~~ |
| com.amazonaws:aws-java-sdk-core: | com.google.protobuf:protobuf-java:3.21.7 *(from 3.20.1)* | ~~com.amazonaws:aws-java-sdk-kinesis:1.12.228~~ |
| com.amazonaws:aws-java-sdk-kinesis: | com.squareup.wire:wire-compiler:4.4.2 *(from 4.3.0)* | ~~io.netty:netty-buffer:4.1.77.Final~~ |
| com.fasterxml.jackson.core:jackson-annotations: | com.squareup.wire:wire-schema:4.4.2 *(from 4.3.0)* | ~~io.netty:netty-codec-http:4.1.77.Final~~ |
| com.fasterxml.jackson.core:jackson-core: | org.apache.avro:avro:1.11.1 *(from 1.11.0)* | ~~io.netty:netty-codec:4.1.77.Final~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.jetbrains.kotlin:kotlin-bom:1.7.10 *(from 1.4.32)* | ~~io.netty:netty-common:4.1.77.Final~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* | ~~io.netty:netty-handler:4.1.77.Final~~ |
| io.netty:netty-bom:4.1.84.Final | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* | ~~io.netty:netty-transport-native-epoll:4.1.77.Final~~ |
| io.netty:netty-buffer: |  | ~~io.netty:netty-transport-native-kqueue:4.1.77.Final~~ |
| io.netty:netty-codec-http: |  | ~~io.netty:netty-transport-native-unix-common:4.1.77.Final~~ |
| io.netty:netty-codec: |  | ~~io.netty:netty-transport:4.1.77.Final~~ |
| io.netty:netty-common: |  |  |
| io.netty:netty-handler: |  |  |
| io.netty:netty-transport-native-epoll: |  |  |
| io.netty:netty-transport-native-kqueue: |  |  |
| io.netty:netty-transport-native-unix-common: |  |  |
| io.netty:netty-transport: |  |  |
| org.apache.kafka:kafka-clients:2.8.2 |  |  |

### interlok-aws-kinesis-sdk ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-bom:1.12.319 | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* | ~~com.amazonaws:aws-java-sdk-core:1.12.228~~ |
| com.amazonaws:aws-java-sdk-core: | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* | ~~com.amazonaws:aws-java-sdk-kinesis:1.12.228~~ |
| com.amazonaws:aws-java-sdk-kinesis: | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-bom:1.12.319 | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* | ~~com.amazonaws:aws-java-sdk-core:1.12.228~~ |
| com.amazonaws:aws-java-sdk-core: | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* | ~~com.amazonaws:aws-java-sdk-kms:1.12.228~~ |
| com.amazonaws:aws-java-sdk-kms: | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-s3 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-bom:1.12.319 | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* | ~~com.amazonaws:aws-java-sdk-core:1.12.228~~ |
| com.amazonaws:aws-java-sdk-core: | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* | ~~com.amazonaws:aws-java-sdk-s3:1.12.228~~ |
| com.amazonaws:aws-java-sdk-s3: | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sns ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-bom:1.12.319 | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* | ~~com.amazonaws:aws-java-sdk-core:1.12.228~~ |
| com.amazonaws:aws-java-sdk-core: | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* | ~~com.amazonaws:aws-java-sdk-sns:1.12.228~~ |
| com.amazonaws:aws-java-sdk-sns: | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sqs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:amazon-sqs-java-messaging-lib:1.1.0 *(from 1.0.8)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-core:1.12.319 *(from 1.12.228)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.amazonaws:aws-java-sdk-sqs:1.12.319 *(from 1.12.228)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-azure-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.azure:azure-identity:1.5.5 *(from 1.5.1)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.azure:azure-storage-file-datalake:12.13.0 *(from 12.10.0)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-xml: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.datatype:jackson-datatype-jsr310: | com.google.code.gson:gson:2.9.1 *(from 2.9.0)* |  |
| io.netty:netty-resolver-dns:4.1.84.Final | com.microsoft.azure:msal4j:1.13.2 *(from 1.12.0)* |  |
| org.codehaus.woodstox:stax2-api:4.2.1 | com.microsoft.graph:microsoft-graph:5.36.0 *(from 2.5.0)* |  |
|  | com.squareup.okhttp3:okhttp:4.10.0 *(from 4.9.3)* |  |
|  | com.squareup.okio:okio:3.2.0 *(from 3.1.0)* |  |
|  | io.netty:netty-codec-http2:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec-http:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-handler:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-azure-cosmosdb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-azure-datalake ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-azure-mail ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-azure-onedrive ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-cassandra ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.datastax.cassandra:cassandra-driver-core:3.11.3 *(from 3.11.1)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.datastax.cassandra:cassandra-driver-mapping:3.11.3 *(from 3.11.1)* |  |
|  | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | io.netty:netty-codec:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-handler:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-client ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-client-jmx ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.apache.logging.log4j:log4j-slf4j2-impl:2.19.0 | org.apache.logging.log4j:log4j-1.2-api:2.19.0 *(from 2.17.2)* | ~~org.apache.logging.log4j:log4j-slf4j-impl:2.17.2~~ |
|  | org.apache.logging.log4j:log4j-api:2.19.0 *(from 2.17.2)* |  |
|  | org.apache.logging.log4j:log4j-core:2.19.0 *(from 2.17.2)* |  |
|  | org.eclipse.jetty.aggregate:jetty-all:9.4.49.v20220914 *(from 9.4.46.v20220331)* |  |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:jul-to-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.4 *(from 0.2.1)* |  |
|  | net.sf.saxon:Saxon-HE:11.4 *(from 11.3)* |  |
|  | org.apache.activemq:activemq-client:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.commons:commons-text:1.10.0 *(from 1.9)* |  |
|  | org.eclipse.jetty.aggregate:jetty-all:9.4.49.v20220914 *(from 9.4.46.v20220331)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-csv ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-csv-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-csv-schema ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-edi-legacy ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-edi-stream ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-ehcache ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-elastic-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | joda-time:joda-time:2.12.0 *(from 2.10.14)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: | org.apache.logging.log4j:log4j-api:2.19.0 *(from 2.17.2)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: | org.elasticsearch:elasticsearch:7.17.6 *(from 7.15.1)* |  |
| org.apache.lucene:lucene-core:8.11.1 | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
| org.elasticsearch:elasticsearch-x-content:7.17.6 | org.yaml:snakeyaml:1.33 *(from 1.30)* |  |

### interlok-elastic-rest ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | joda-time:joda-time:2.12.0 *(from 2.10.14)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: | org.apache.logging.log4j:log4j-api:2.19.0 *(from 2.17.2)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: | org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.17.6 *(from 7.15.1)* |  |
| org.elasticsearch:elasticsearch-x-content:7.17.6 | org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.6 *(from 7.15.1)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
|  | org.yaml:snakeyaml:1.33 *(from 1.30)* |  |

### interlok-elastic-sdk ###
| Initial Dependencies |
| -------- |
| co.elastic.clients:elasticsearch-java:7.17.6 |
| com.fasterxml.jackson.core:jackson-databind: |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |
| com.fasterxml.jackson:jackson-bom:2.13.4.20221013 |
| com.jayway.jsonpath:json-path:2.7.0 |
| commons-collections:commons-collections:3.2.2 |
| joda-time:joda-time:2.12.0 |
| org.apache.logging.log4j:log4j-api:2.19.0 |
| org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.6 |
| org.elasticsearch:elasticsearch-x-content:7.17.6 |
| org.slf4j:slf4j-api:2.0.3 |
| org.yaml:snakeyaml:1.33 |

### interlok-excel ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-exec ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-expressions ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-failover ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-filesystem ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.tika:tika-core:2.5.0 *(from 2.4.0)* |  |
|  | org.json:json:20220924 *(from 20220320)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-flyway ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.flywaydb:flyway-core:8.5.13 *(from 8.5.11)* |  |

### interlok-gcloud-pubsub ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | com.google.cloud:google-cloud-pubsub:1.120.20 *(from 1.118.0)* |  |
|  | com.google.code.gson:gson:2.9.1 *(from 2.9.0)* |  |
|  | com.google.protobuf:protobuf-java-util:3.21.7 *(from 3.20.1)* |  |
|  | com.google.protobuf:protobuf-java:3.21.7 *(from 3.20.1)* |  |
|  | io.grpc:grpc-alts:1.50.0 *(from 1.46.0)* |  |
|  | io.grpc:grpc-auth:1.50.0 *(from 1.46.0)* |  |
|  | io.grpc:grpc-netty:1.50.0 *(from 1.46.0)* |  |
|  | io.grpc:grpc-protobuf:1.50.0 *(from 1.46.0)* |  |
|  | io.grpc:grpc-stub:1.50.0 *(from 1.46.0)* |  |
|  | io.netty:netty-codec-http2:4.1.82.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec-http:4.1.82.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec:4.1.82.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.82.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-handler:4.1.82.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.82.Final *(from 4.1.77.Final)* |  |

### interlok-hpcc ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jclouds-aws-sts ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jclouds-blobstore ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jclouds-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jdbc ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jms-oracleaq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jms-sonicmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jmx-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.activemq:activemq-client:5.17.2 *(from 5.17.1)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
|  | org.springframework:spring-aop:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-beans:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-context:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-core:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-jms:5.3.23 *(from 5.3.20)* |  |

### interlok-jmx-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.netty:netty-buffer:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec-http:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-codec:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-common:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-handler:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | org.apache.qpid:proton-j:0.34.0 *(from 0.33.10)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
|  | org.springframework:spring-aop:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-beans:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-context:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-core:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-jms:5.3.23 *(from 5.3.20)* |  |

### interlok-jmx-jms-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
|  | org.springframework:spring-aop:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-beans:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-context:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-core:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-jms:5.3.23 *(from 5.3.20)* |  |

### interlok-jmx-jms-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.activemq:activemq-amqp:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-broker:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-jaas:5.17.2 *(from 5.17.1)* |  |
|  | org.apache.activemq:activemq-kahadb-store:5.17.2 *(from 5.17.1)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
|  | org.springframework:spring-aop:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-beans:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-context:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-core:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-jms:5.3.23 *(from 5.3.20)* |  |

### interlok-jmx-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.16.0 *(from 10.14.0)* |  |
|  | com.solacesystems:sol-jcsmp:10.16.0 *(from 10.14.0)* |  |
|  | com.solacesystems:sol-jms:10.16.0 *(from 10.14.0)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
|  | org.springframework:spring-aop:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-beans:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-context:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-core:5.3.23 *(from 5.3.20)* |  |
|  | org.springframework:spring-jms:5.3.23 *(from 5.3.20)* |  |

### interlok-jmx-sonicmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jolokia ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.eclipse.jetty.aggregate:jetty-all:9.4.49.v20220914 *(from 9.4.46.v20220331)* |  |

### interlok-jq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | net.thisptr:jackson-jq-extra:1.0.0-preview.20220705 *(from 1.0.0-preview.20210928)* |  |
|  | net.thisptr:jackson-jq:1.0.0-preview.20220705 *(from 1.0.0-preview.20210928)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jruby ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jruby:jruby:9.3.8.0 *(from 9.3.4.0)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jslt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | com.schibsted.spt.data:jslt:0.1.13 *(from 0.1.12)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.core:jackson-core: | org.json:json:20220924 *(from 20220320)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: | xom:xom:1.3.8 *(from 1.3.7)* |  |

### interlok-json-streaming ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.google.code.gson:gson:2.9.1 *(from 2.9.0)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-json-web-token ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | org.json:json:20220924 *(from 20220320)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-jsr107-cache ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-kafka ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | io.netty:netty-codec:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-handler:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.84.Final *(from 4.1.77.Final)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-kie ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.drools:drools-compiler:7.73.0.Final *(from 7.70.0.Final)* |  |
|  | org.drools:drools-core:7.73.0.Final *(from 7.70.0.Final)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-licensing ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-licensing-demo ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-logging ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.logging.log4j:log4j-api:2.19.0 *(from 2.17.2)* |  |
|  | org.apache.logging.log4j:log4j-core:2.19.0 *(from 2.17.2)* |  |

### interlok-mongodb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-mqtt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-msmq-javonet ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-nats ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.nats:jnats:2.16.1 *(from 2.15.1)* |  |

### interlok-oauth-azure ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.code.gson:gson:2.9.1 *(from 2.9.0)* |  |
|  | com.nimbusds:nimbus-jose-jwt:9.25.4 *(from 9.22)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-oauth-gcloud ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-core:2.13.4 *(from 2.13.3)* |  |
|  | com.google.auth:google-auth-library-oauth2-http:1.11.0 *(from 1.7.0)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-oauth-generic ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-oauth-salesforce ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-okhttp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.squareup.okhttp3:okhttp:4.10.0 *(from 4.9.3)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-pdf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.apache.xmlgraphics:batik-extension:1.15 | org.apache.pdfbox:fontbox:2.0.27 *(from 2.0.26)* |  |
| org.apache.xmlgraphics:batik-transcoder:1.15 | org.apache.pdfbox:pdfbox-tools:2.0.27 *(from 2.0.26)* |  |
|  | org.apache.pdfbox:pdfbox:2.0.27 *(from 2.0.26)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-pgp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-profiler ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-rabbitmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.16.0 *(from 5.14.2)* |  |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-rest-metrics-jvm ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-core:1.9.5 *(from 1.9.0)* |  |

### interlok-rest-provider-datadog ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-registry-datadog:1.9.5 *(from 1.9.0)* |  |

### interlok-rest-provider-prometheus ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-registry-prometheus:1.9.5 *(from 1.9.0)* |  |

### interlok-sap ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-service-tester ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-service-tester-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.json:json:20220924 *(from 20220320)* |  |
|  | org.skyscreamer:jsonassert:1.5.1 *(from 1.5.0)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-service-tester-wiremock ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.13.4.20221013 *(from 2.13.3)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.github.tomakehurst:wiremock-jre8:2.34.0 *(from 2.33.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
| org.eclipse.jetty:jetty-bom:9.4.48.v20220622 |  |  |

### interlok-service-tester-xml ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.16.0 *(from 10.14.0)* |  |
|  | com.solacesystems:sol-jcsmp:10.16.0 *(from 10.14.0)* |  |
|  | com.solacesystems:sol-jms:10.16.0 *(from 10.14.0)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-sshtunnel ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.4 *(from 0.2.1)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-stax ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-swift ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.prowidesoftware:pw-swift-core:SRU2021-9.2.18 *(from SRU2021-9.2.13)* |  |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-tibco ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-triggered ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-vcs-git ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.4 *(from 0.2.1)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-webservice-cxf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.cxf:cxf-rt-frontend-jaxws:3.5.4 *(from 3.5.2)* |  |
|  | org.apache.cxf:cxf-rt-transports-http:3.5.4 *(from 3.5.2)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-webspheremq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.3.0.1 *(from 9.2.5.0)* |  |
|  | org.slf4j:jcl-over-slf4j:2.0.3 *(from 1.7.36)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-work-unit ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-xa-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-xa-atomikos ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-xa-jms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-xa-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.16.0 *(from 10.14.0)* |  |
|  | com.solacesystems:sol-jcsmp:10.16.0 *(from 10.14.0)* |  |
|  | com.solacesystems:sol-jms:10.16.0 *(from 10.14.0)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-xa-tibco ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-xa-wmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.3.0.1 *(from 9.2.5.0)* |  |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |

### interlok-xml-security ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.3 *(from 1.7.36)* |  |
