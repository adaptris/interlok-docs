## Version 4.5.0 ##

### interlok-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.activemq:activemq-amqp:5.17.1 *(from 5.16.3)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | org.apache.activemq:activemq-broker:5.17.1 *(from 5.16.3)* |  |
|  | org.apache.activemq:activemq-client:5.17.1 *(from 5.16.3)* |  |
|  | org.apache.activemq:activemq-jaas:5.17.1 *(from 5.16.3)* |  |
|  | org.apache.activemq:activemq-kahadb-store:5.17.1 *(from 5.16.3)* |  |
|  | org.apache.activemq:activemq-mqtt:5.17.1 *(from 5.16.3)* |  |
|  | org.apache.activemq:activemq-spring:5.17.1 *(from 5.16.3)* |  |
|  | org.apache.activemq:activemq-stomp:5.17.1 *(from 5.16.3)* |  |
|  | org.springframework:spring-beans:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-context:5.3.20 *(from 5.3.15)* |  |

### interlok-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.14.2 *(from 5.14.1)* |  |
|  | io.netty:netty-buffer:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-codec-http:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-codec:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-common:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-handler:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | org.apache.qpid:qpid-jms-client:1.6.0 *(from 1.5.0)* |  |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-apache-geode ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | org.apache.geode:geode-core:1.14.4 *(from 1.14.3)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | org.apache.shiro:shiro-core:1.9.0 *(from 1.8.0)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |
| org.jgroups:jgroups:4.2.4.Final |  |  |
| org.springframework:spring-web:5.3.20 |  |  |

### interlok-apache-http ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-apache-http-async ###
| Initial Dependencies |
| -------- |
| org.apache.httpcomponents:httpasyncclient:4.1.5 |
| org.apache.httpcomponents:httpclient:4.5.13 |
| org.slf4j:slf4j-api:1.7.36 |

### interlok-apache-http5 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents.client5:httpclient5:5.1.3 *(from 5.1.2)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-artemis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.jgroups:jgroups:4.2.4.Final | io.netty:netty-buffer:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-codec-http:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-codec:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-common:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-handler:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | org.apache.activemq:artemis-jms-server:2.22.0 *(from 2.20.0)* |  |
|  | org.apache.activemq:artemis-server:2.22.0 *(from 2.20.0)* |  |

### interlok-as400 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-aws-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:aws-java-sdk-core:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-sts:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-aws-kinesis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:amazon-kinesis-client:1.14.8 *(from 1.14.7)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:amazon-kinesis-producer:0.14.12 *(from 0.14.10)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | com.amazonaws:aws-java-sdk-core:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | com.amazonaws:aws-java-sdk-kinesis:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* |  |
| com.squareup.wire:wire-compiler:4.3.0 | com.google.protobuf:protobuf-java:3.20.1 *(from 3.19.4)* |  |
| com.squareup.wire:wire-schema:4.3.0 | io.netty:netty-buffer:4.1.77.Final *(from 4.1.73.Final)* |  |
| org.jetbrains.kotlin:kotlin-bom:1.4.32 | io.netty:netty-codec-http:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-codec:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-common:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-handler:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-aws-kinesis-sdk ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:aws-java-sdk-core:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-kinesis:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-aws-kms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:aws-java-sdk-core:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-kms:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-aws-s3 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:aws-java-sdk-core:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-s3:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-aws-sns ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:aws-java-sdk-core:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-sns:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-aws-sqs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:aws-java-sdk-core:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-sqs:1.12.228 *(from 1.12.150)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-azure-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.azure:azure-identity:1.5.1 *(from 1.4.3)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | com.azure:azure-storage-file-datalake:12.10.0 *(from 12.7.3)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-xml: | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* | ~~com.fasterxml.jackson.dataformat:jackson-dataformat-xml:2.13.1~~ |
| com.fasterxml.jackson.datatype:jackson-datatype-jsr310: | com.microsoft.azure:msal4j:1.12.0 *(from 1.11.0)* | ~~com.fasterxml.jackson.datatype:jackson-datatype-jsr310:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | io.netty:netty-codec-http2:4.1.77.Final *(from 4.1.73.Final)* |  |
| com.google.code.gson:gson:2.9.0 | io.netty:netty-codec-http:4.1.77.Final *(from 4.1.73.Final)* |  |
| com.squareup.okhttp3:okhttp:4.9.3 | io.netty:netty-codec:4.1.77.Final *(from 4.1.73.Final)* |  |
| com.squareup.okio:okio:3.1.0 | io.netty:netty-handler-proxy:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-handler:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-azure-cosmosdb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: |  | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-azure-datalake ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-azure-mail ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-azure-onedrive ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-cassandra ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.datastax.cassandra:cassandra-driver-core:3.11.1 *(from 3.11.0)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | com.datastax.cassandra:cassandra-driver-mapping:3.11.1 *(from 3.11.0)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* |  |
|  | io.netty:netty-codec:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-handler:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-client ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-client-jmx ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.logging.log4j:log4j-1.2-api:2.17.2 *(from 2.17.1)* |  |
|  | org.apache.logging.log4j:log4j-api:2.17.2 *(from 2.17.1)* |  |
|  | org.apache.logging.log4j:log4j-core:2.17.2 *(from 2.17.1)* |  |
|  | org.apache.logging.log4j:log4j-slf4j-impl:2.17.2 *(from 2.17.1)* |  |
|  | org.eclipse.jetty.aggregate:jetty-all:9.4.46.v20220331 *(from 9.4.44.v20210927)* |  |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:jul-to-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.1 *(from 0.1.72)* |  |
|  | net.sf.saxon:Saxon-HE:11.3 *(from 10.6)* |  |
|  | org.apache.activemq:activemq-client:5.17.1 *(from 5.16.3)* |  |
|  | org.eclipse.jetty.aggregate:jetty-all:9.4.46.v20220331 *(from 9.4.44.v20210927)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-csv ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-csv-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-csv-schema ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-edi-legacy ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-edi-stream ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-ehcache ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-elastic-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | joda-time:joda-time:2.10.14 *(from 2.10.13)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.apache.logging.log4j:log4j-api:2.17.2 *(from 2.17.1)* | ~~commons-codec:commons-codec:1.15~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~org.apache.httpcomponents:httpclient:4.5.13~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  | ~~org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.15.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  | ~~org.elasticsearch.client:elasticsearch-rest-high-level-client:7.15.1~~ |
| org.elasticsearch:elasticsearch:7.15.1 |  |  |

### interlok-elastic-rest ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | joda-time:joda-time:2.10.14 *(from 2.10.13)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.apache.logging.log4j:log4j-api:2.17.2 *(from 2.17.1)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-excel ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-exec ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-expressions ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-failover ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-filesystem ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.hierynomus:smbj:0.11.5 *(from 0.11.3)* |  |
|  | org.apache.tika:tika-core:2.4.0 *(from 2.2.1)* |  |
|  | org.json:json:20220320 *(from 20211205)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-flyway ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.flywaydb:flyway-core:8.5.11 *(from 8.4.3)* |  |

### interlok-gcloud-pubsub ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.google.cloud:google-cloud-pubsub:1.118.0 *(from 1.115.1)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | com.google.code.gson:gson:2.9.0 *(from 2.8.9)* |  |
|  | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* |  |
|  | com.google.protobuf:protobuf-java-util:3.20.1 *(from 3.19.3)* |  |
|  | com.google.protobuf:protobuf-java:3.20.1 *(from 3.19.3)* |  |
|  | io.grpc:grpc-alts:1.46.0 *(from 1.44.0)* |  |
|  | io.grpc:grpc-auth:1.46.0 *(from 1.44.0)* |  |
|  | io.grpc:grpc-netty:1.46.0 *(from 1.44.0)* |  |
|  | io.grpc:grpc-protobuf:1.46.0 *(from 1.44.0)* |  |
|  | io.grpc:grpc-stub:1.46.0 *(from 1.44.0)* |  |
|  | io.netty:netty-codec-http2:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-codec-http:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-codec:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-handler:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.77.Final *(from 4.1.73.Final)* |  |

### interlok-hpcc ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-jclouds-aws-sts ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.jclouds.api:sts:2.5.0 *(from 2.4.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-jclouds-blobstore ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.jclouds:jclouds-blobstore:2.5.0 *(from 2.4.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-jclouds-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* |  |
|  | org.apache.jclouds:jclouds-core:2.5.0 *(from 2.4.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-jdbc ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-jms-oracleaq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-jms-sonicmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.32)* |  |

### interlok-jmx-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.activemq:activemq-client:5.17.1 *(from 5.16.3)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |
|  | org.springframework:spring-aop:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-beans:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-context:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-core:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-jms:5.3.20 *(from 5.3.15)* |  |

### interlok-jmx-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.netty:netty-buffer:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-codec-http:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-codec:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-common:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-handler:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | io.netty:netty-transport:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | org.apache.qpid:qpid-jms-client:1.6.0 *(from 1.5.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |
|  | org.springframework:spring-aop:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-beans:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-context:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-core:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-jms:5.3.20 *(from 5.3.15)* |  |

### interlok-jmx-jms-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |
|  | org.springframework:spring-aop:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-beans:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-context:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-core:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-jms:5.3.20 *(from 5.3.15)* |  |

### interlok-jmx-jms-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | org.apache.activemq:activemq-amqp:5.17.1 *(from 5.16.3)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.apache.activemq:activemq-broker:5.17.1 *(from 5.16.3)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | org.apache.activemq:activemq-jaas:5.17.1 *(from 5.16.3)* |  |
|  | org.apache.activemq:activemq-kahadb-store:5.17.1 *(from 5.16.3)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |
|  | org.springframework:spring-aop:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-beans:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-context:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-core:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-jms:5.3.20 *(from 5.3.15)* |  |

### interlok-jmx-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.14.0 *(from 10.13.0)* |  |
|  | com.solacesystems:sol-jcsmp:10.14.0 *(from 10.13.0)* |  |
|  | com.solacesystems:sol-jms:10.14.0 *(from 10.13.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |
|  | org.springframework:spring-aop:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-beans:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-context:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-core:5.3.20 *(from 5.3.15)* |  |
|  | org.springframework:spring-jms:5.3.20 *(from 5.3.15)* |  |

### interlok-jmx-sonicmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.32)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.32)* |  |

### interlok-jolokia ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.eclipse.jetty.aggregate:jetty-all:9.4.46.v20220331 *(from 9.4.44.v20210927)* |  |

### interlok-jq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-jruby ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jruby:jruby:9.3.4.0 *(from 9.3.3.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-jslt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.schibsted.spt.data:jslt:0.1.12 *(from 0.1.11)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.bazaarvoice.jolt:jolt-core:0.1.7 *(from 0.1.5)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | com.bazaarvoice.jolt:json-utils:0.1.7 *(from 0.1.5)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | com.flipkart.zjsonpatch:zjsonpatch:0.4.12 *(from 0.4.11)* | ~~com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.13.1~~ |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* | ~~com.github.everit-org.json-schema:org.everit.json.schema:1.14.0~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | org.json:json:20220320 *(from 20211205)* |  |
| com.github.erosb:everit-json-schema:1.14.1 | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-json-streaming ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.google.code.gson:gson:2.9.0 *(from 2.8.9)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: |  | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-json-web-token ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | io.jsonwebtoken:jjwt-api:0.11.5 *(from 0.11.2)* | ~~com.fasterxml.jackson.core:jackson-databind:2.12.5~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | io.jsonwebtoken:jjwt-impl:0.11.5 *(from 0.11.2)* |  |
|  | io.jsonwebtoken:jjwt-jackson:0.11.5 *(from 0.11.2)* |  |
|  | org.json:json:20220320 *(from 20211205)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-jsr107-cache ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-kafka ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | io.netty:netty-codec:4.1.77.Final *(from 4.1.73.Final)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | io.netty:netty-handler:4.1.77.Final *(from 4.1.73.Final)* |  |
| org.apache.zookeeper:zookeeper:3.8.0 | io.netty:netty-transport-native-epoll:4.1.77.Final *(from 4.1.73.Final)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-kie ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.drools:drools-compiler:7.70.0.Final *(from 7.64.0.Final)* |  |
|  | org.drools:drools-core:7.70.0.Final *(from 7.64.0.Final)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-licensing ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.32)* |  |

### interlok-licensing-demo ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.32)* |  |

### interlok-logging ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.logging.log4j:log4j-api:2.17.2 *(from 2.17.1)* |  |
|  | org.apache.logging.log4j:log4j-core:2.17.2 *(from 2.17.1)* |  |

### interlok-mongodb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.mongodb:mongodb-driver:3.12.11 *(from 3.12.10)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-mqtt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-msmq-javonet ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-nats ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.nats:jnats:2.15.1 *(from 2.13.2)* |  |

### interlok-oauth-azure ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.google.code.gson:gson:2.9.0 | com.nimbusds:nimbus-jose-jwt:9.22 *(from 9.16.1)* |  |
|  | net.minidev:json-smart:2.4.8 *(from 2.4.7)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-oauth-gcloud ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-core:2.13.3 *(from 2.13.1)* |  |
|  | com.google.auth:google-auth-library-oauth2-http:1.7.0 *(from 1.4.0)* |  |
|  | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-oauth-generic ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-oauth-salesforce ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-okhttp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-pdf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* |  |
|  | org.apache.pdfbox:fontbox:2.0.26 *(from 2.0.25)* |  |
|  | org.apache.pdfbox:pdfbox-tools:2.0.26 *(from 2.0.25)* |  |
|  | org.apache.pdfbox:pdfbox:2.0.26 *(from 2.0.25)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-pgp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-profiler ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.aspectj:aspectjrt:1.9.9.1 *(from 1.9.7)* |  |
|  | org.aspectj:aspectjtools:1.9.9.1 *(from 1.9.7)* |  |
|  | org.aspectj:aspectjweaver:1.9.9.1 *(from 1.9.7)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-proxy ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents.client5:httpclient5:5.1.3 *(from 5.1.2)* |  |

### interlok-rabbitmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.14.2 *(from 5.14.1)* |  |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-rest-metrics-jvm ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-core:1.9.0 *(from 1.8.2)* |  |

### interlok-rest-provider-datadog ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-registry-datadog:1.9.0 *(from 1.8.2)* |  |

### interlok-rest-provider-prometheus ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-registry-prometheus:1.9.0 *(from 1.8.2)* |  |

### interlok-sap ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-service-tester ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-service-tester-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | org.json:json:20220320 *(from 20211205)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-service-tester-wiremock ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.github.tomakehurst:wiremock-jre8:2.33.2 *(from 2.32.0)* | ~~com.fasterxml.jackson.core:jackson-annotations:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-core: | com.google.guava:guava:31.1-jre *(from 31.0.1-jre)* | ~~com.fasterxml.jackson.core:jackson-core:2.13.1~~ |
| com.fasterxml.jackson.core:jackson-databind: | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* | ~~com.fasterxml.jackson.core:jackson-databind:2.13.1~~ |
| com.fasterxml.jackson:jackson-bom:2.13.3 |  |  |

### interlok-service-tester-xml ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.14.0 *(from 10.13.0)* |  |
|  | com.solacesystems:sol-jcsmp:10.14.0 *(from 10.13.0)* |  |
|  | com.solacesystems:sol-jms:10.14.0 *(from 10.13.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-sshtunnel ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.1 *(from 0.1.72)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-stax ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-swift ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.prowidesoftware:pw-swift-core:SRU2021-9.2.13 *(from SRU2021-9.2.11)* |  |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-tibco ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-triggered ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-vcs-git ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.1 *(from 0.1.72)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-webservice-cxf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.cxf:cxf-rt-frontend-jaxws:3.5.2 *(from 3.5.0)* |  |
|  | org.apache.cxf:cxf-rt-transports-http:3.5.2 *(from 3.5.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-webspheremq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.2.5.0 *(from 9.2.4.0)* |  |
|  | org.slf4j:jcl-over-slf4j:1.7.36 *(from 1.7.35)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-work-unit ###
| Initial Dependencies |
| -------- |
| org.slf4j:slf4j-api:1.7.36 |

### interlok-xa-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-xa-atomikos ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.awaitility:awaitility:4.2.0 *(from 4.1.1)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-xa-jms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-xa-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.14.0 *(from 10.13.0)* |  |
|  | com.solacesystems:sol-jcsmp:10.14.0 *(from 10.13.0)* |  |
|  | com.solacesystems:sol-jms:10.14.0 *(from 10.13.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-xa-tibco ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-xa-wmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.2.5.0 *(from 9.2.4.0)* |  |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.35)* |  |

### interlok-xml-security ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:1.7.36 *(from 1.7.32)* |  |
