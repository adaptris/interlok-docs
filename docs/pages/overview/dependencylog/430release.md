## Version 4.3.0 ##

### interlok-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |
|  | org.apache.activemq:activemq-amqp:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-broker:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-client:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-jaas:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-kahadb-store:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-mqtt:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-spring:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-stomp:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.qpid:proton-j:0.33.10 *(from 0.33.8)* |  |
|  | org.springframework:spring-beans:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-context:5.3.12 *(from 5.3.9)* |  |

### interlok-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.slf4j:jcl-over-slf4j:1.7.32 | com.rabbitmq:amqp-client:5.13.1 *(from 5.13.0)* |  |
|  | io.netty:netty-buffer:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec-http:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-common:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-handler:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | org.apache.qpid:proton-j:0.33.10 *(from 0.33.8)* |  |
|  | org.apache.qpid:qpid-jms-client:1.3.0 *(from 1.1.0)* |  |

### interlok-apache-geode ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* | ~~org.apache.httpcomponents:httpclient:4.5.13~~ |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | org.apache.geode:geode-core:1.14.0 *(from 1.13.4)* |  |
|  | org.apache.shiro:shiro-core:1.8.0 *(from 1.7.1)* |  |

### interlok-apache-http5 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents.client5:httpclient5:5.1.1 *(from 5.1)* |  |

### interlok-artemis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.netty:netty-buffer:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec-http:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-common:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-handler:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | org.apache.activemq:artemis-jms-server:2.19.0 *(from 2.18.0)* |  |
|  | org.apache.activemq:artemis-server:2.19.0 *(from 2.18.0)* |  |

### interlok-aws-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.amazonaws:aws-java-sdk-core:1.12.107 *(from 1.12.46)* |  |
|  | com.amazonaws:aws-java-sdk-sts:1.12.107 *(from 1.12.46)* |  |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.0 *(from 2.12.4)* |  |

### interlok-aws-kinesis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.amazonaws:amazon-kinesis-producer:0.14.10 *(from 0.14.9)* |  |
|  | com.amazonaws:aws-java-sdk-core:1.12.107 *(from 1.12.46)* |  |
|  | com.amazonaws:aws-java-sdk-kinesis:1.12.107 *(from 1.12.46)* |  |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.0 *(from 2.12.4)* |  |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |
|  | com.google.protobuf:protobuf-java:3.19.1 *(from 3.17.3)* |  |
|  | io.netty:netty-buffer:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec-http:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-common:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-handler:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | org.apache.avro:avro:1.11.0 *(from 1.10.2)* |  |

### interlok-aws-kinesis-sdk ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.amazonaws:aws-java-sdk-core:1.12.107 *(from 1.12.46)* |  |
|  | com.amazonaws:aws-java-sdk-kinesis:1.12.107 *(from 1.12.46)* |  |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.0 *(from 2.12.4)* |  |

### interlok-aws-kms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.amazonaws:aws-java-sdk-core:1.12.107 *(from 1.12.46)* |  |
|  | com.amazonaws:aws-java-sdk-kms:1.12.107 *(from 1.12.46)* |  |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.0 *(from 2.12.4)* |  |

### interlok-aws-s3 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.amazonaws:aws-java-sdk-core:1.12.107 *(from 1.12.46)* |  |
|  | com.amazonaws:aws-java-sdk-s3:1.12.107 *(from 1.12.46)* |  |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.0 *(from 2.12.4)* |  |

### interlok-aws-sns ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.amazonaws:aws-java-sdk-core:1.12.107 *(from 1.12.46)* |  |
|  | com.amazonaws:aws-java-sdk-sns:1.12.107 *(from 1.12.46)* |  |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.0 *(from 2.12.4)* |  |

### interlok-aws-sqs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.amazonaws:aws-java-sdk-core:1.12.107 *(from 1.12.46)* |  |
|  | com.amazonaws:aws-java-sdk-sqs:1.12.107 *(from 1.12.46)* |  |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.13.0 *(from 2.12.4)* |  |

### interlok-azure-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.azure:azure-identity:1.3.7 *(from 1.3.5)* |  |
|  | com.azure:azure-storage-file-datalake:12.7.1 *(from 12.6.0)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-xml:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.datatype:jackson-datatype-jsr310:2.13.0 *(from 2.12.4)* |  |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |
|  | io.netty:netty-codec-http2:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec-http:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-handler:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.70.Final *(from 4.1.66.Final)* |  |

### interlok-azure-cosmosdb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |

### interlok-cassandra ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |
|  | io.netty:netty-codec:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-handler:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.70.Final *(from 4.1.66.Final)* |  |

### interlok-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.commons:commons-pool2:2.11.1 *(from 2.11.0)* | ~~javax:javaee-api:8.0.1~~ |
|  | org.eclipse.jetty.aggregate:jetty-all:9.4.44.v20210927 *(from 9.4.43.v20210629)* |  |

### interlok-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| jakarta.jms:jakarta.jms-api:2.0.3 | com.github.mwiede:jsch:0.1.69 *(from 0.1.64)* | ~~javax:javaee-api:8.0.1~~ |
|  | io.github.classgraph:classgraph:4.8.116 *(from 4.8.60)* | ~~org.apache.geronimo.specs:geronimo-jms_2.0_spec:1.0-alpha-2~~ |
|  | net.sf.saxon:Saxon-HE:10.6 *(from 10.5)* |  |
|  | org.apache.activemq:activemq-client:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.commons:commons-pool2:2.11.1 *(from 2.11.0)* |  |
|  | org.eclipse.jetty.aggregate:jetty-all:9.4.44.v20210927 *(from 9.4.43.v20210629)* |  |
|  | org.hibernate.validator:hibernate-validator:6.1.7.Final *(from 6.1.6.Final)* |  |

### interlok-core-apt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  |  | ~~javax:javaee-api:8.0.1~~ |

### interlok-csv-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |

### interlok-elastic-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | joda-time:joda-time:2.10.13 *(from 2.10.10)* |  |
|  | org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.15.1 *(from 7.13.4)* |  |
|  | org.elasticsearch.client:elasticsearch-rest-high-level-client:7.15.1 *(from 7.13.4)* |  |

### interlok-elastic-rest ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | joda-time:joda-time:2.10.13 *(from 2.10.10)* |  |
|  | org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.15.1 *(from 7.13.4)* |  |
|  | org.elasticsearch.client:elasticsearch-rest-high-level-client:7.15.1 *(from 7.13.4)* |  |

### interlok-filesystem ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.hierynomus:smbj:0.11.3 *(from 0.11.1)* |  |
|  | org.apache.tika:tika-core:2.1.0 *(from 2.0.0)* |  |

### interlok-flyway ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.flywaydb:flyway-core:8.0.3 *(from 7.13.0)* |  |

### interlok-gcloud-pubsub ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| io.netty:netty-handler-proxy:4.1.70.Final | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.google.cloud:google-cloud-pubsub:1.114.7 *(from 1.114.0)* |  |
|  | com.google.code.gson:gson:2.8.9 *(from 2.8.7)* |  |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |
|  | com.google.protobuf:protobuf-java-util:3.19.1 *(from 3.17.3)* |  |
|  | com.google.protobuf:protobuf-java:3.19.1 *(from 3.17.3)* |  |
|  | io.grpc:grpc-alts:1.42.0 *(from 1.39.0)* |  |
|  | io.grpc:grpc-auth:1.42.0 *(from 1.39.0)* |  |
|  | io.grpc:grpc-netty:1.42.0 *(from 1.39.0)* |  |
|  | io.grpc:grpc-protobuf:1.42.0 *(from 1.39.0)* |  |
|  | io.grpc:grpc-stub:1.42.0 *(from 1.39.0)* |  |
|  | io.netty:netty-codec-http2:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec-http:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-handler:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.70.Final *(from 4.1.66.Final)* |  |

### interlok-jclouds-aws-sts ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.jclouds.api:sts:2.4.0 *(from 2.3.0)* |  |

### interlok-jclouds-blobstore ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.jclouds:jclouds-blobstore:2.4.0 *(from 2.3.0)* |  |

### interlok-jclouds-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |
|  | org.apache.jclouds:jclouds-core:2.4.0 *(from 2.3.0)* |  |

### interlok-jdbc ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |

### interlok-jmx-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.activemq:activemq-client:5.16.3 *(from 5.16.2)* |  |
|  | org.springframework:spring-aop:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-beans:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-context:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-core:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-jms:5.3.12 *(from 5.3.9)* |  |

### interlok-jmx-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.netty:netty-buffer:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec-http:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-codec:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-common:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-handler:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | org.apache.qpid:proton-j:0.33.10 *(from 0.33.8)* |  |
|  | org.apache.qpid:qpid-jms-client:1.3.0 *(from 1.1.0)* |  |
|  | org.springframework:spring-aop:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-beans:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-context:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-core:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-jms:5.3.12 *(from 5.3.9)* |  |

### interlok-jmx-jms-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.springframework:spring-aop:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-beans:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-context:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-core:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-jms:5.3.12 *(from 5.3.9)* |  |

### interlok-jmx-jms-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | org.apache.activemq:activemq-amqp:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-broker:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-jaas:5.16.3 *(from 5.16.2)* |  |
|  | org.apache.activemq:activemq-kahadb-store:5.16.3 *(from 5.16.2)* |  |
|  | org.springframework:spring-aop:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-beans:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-context:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-core:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-jms:5.3.12 *(from 5.3.9)* |  |

### interlok-jmx-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.12.1 *(from 10.12.0)* |  |
|  | com.solacesystems:sol-jcsmp:10.12.1 *(from 10.12.0)* |  |
|  | com.solacesystems:sol-jms:10.12.1 *(from 10.12.0)* |  |
|  | org.springframework:spring-aop:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-beans:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-context:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-core:5.3.12 *(from 5.3.9)* |  |
|  | org.springframework:spring-jms:5.3.12 *(from 5.3.9)* |  |

### interlok-jolokia ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.eclipse.jetty.aggregate:jetty-all:9.4.44.v20210927 | org.jolokia:jolokia-core:1.7.1 *(from 1.6.2)* |  |
|  | org.jolokia:jolokia-jsr160:1.7.1 *(from 1.6.2)* |  |

### interlok-jq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| net.thisptr:jackson-jq-extra:1.0.0-preview.20210928 | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | net.thisptr:jackson-jq:1.0.0-preview.20210928 *(from 0.0.13)* |  |

### interlok-jruby ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jruby:jruby:9.3.1.0 *(from 9.2.19.0)* |  |

### interlok-jslt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |

### interlok-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.bazaarvoice.jolt:jolt-core:0.1.5 *(from 0.1.1)* |  |
|  | com.bazaarvoice.jolt:json-utils:0.1.5 *(from 0.1.1)* |  |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-yaml:2.13.0 *(from 2.12.4)* |  |
|  | com.github.everit-org.json-schema:org.everit.json.schema:1.14.0 *(from 1.13.0)* |  |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |

### interlok-json-streaming ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.github.jsurfer:jsurfer-core:1.6.2 | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.4)* |  |
| com.google.code.gson:gson:2.8.9 | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | com.github.jsurfer:jsurfer-gson:1.6.2 *(from 1.6.1)* |  |
|  | com.github.jsurfer:jsurfer-jackson:1.6.2 *(from 1.6.1)* |  |
|  | com.github.jsurfer:jsurfer-jsonsimple:1.6.2 *(from 1.6.1)* |  |

### interlok-json-web-token ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-databind:2.12.5 *(from 2.12.1)* |  |

### interlok-kafka ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |
|  | io.netty:netty-codec:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-handler:4.1.70.Final *(from 4.1.66.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.70.Final *(from 4.1.66.Final)* |  |

### interlok-kie ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.drools:drools-compiler:7.61.0.Final *(from 7.59.0.Final)* |  |
|  | org.drools:drools-core:7.61.0.Final *(from 7.59.0.Final)* |  |

### interlok-mongodb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |

### interlok-nats ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.nats:jnats:2.13.1 *(from 2.11.5)* |  |

### interlok-oauth-gcloud ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.4)* |  |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |

### interlok-oauth-generic ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |

### interlok-oauth-salesforce ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.4)* |  |

### interlok-okhttp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.squareup.okhttp3:okhttp:4.9.2 *(from 4.9.1)* |  |

### interlok-pdf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |

### interlok-proxy ###
| Initial Dependencies |
| -------- |
| org.apache.httpcomponents.client5:httpclient5:5.1.1 |

### interlok-rabbitmq ###
| Initial Dependencies |
| -------- |
| com.rabbitmq:amqp-client:5.13.1 |
| org.slf4j:jcl-over-slf4j:1.7.32 |
| org.slf4j:slf4j-api:1.7.32 |

### interlok-rest-metrics-jvm ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-core:1.7.5 *(from 1.7.3)* |  |

### interlok-rest-provider-datadog ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-registry-datadog:1.8.0 *(from 1.7.3)* |  |

### interlok-rest-provider-prometheus ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-registry-prometheus:1.8.0 *(from 1.7.3)* |  |

### interlok-sap ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.ant:ant:1.10.11 *(from 1.10.9)* |  |

### interlok-service-tester-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.5)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.5)* |  |

### interlok-service-tester-wiremock ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-annotations:2.13.0 *(from 2.12.5)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.13.0 *(from 2.12.5)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.13.0 *(from 2.12.5)* |  |
|  | com.google.guava:guava:31.0.1-jre *(from 30.1.1-jre)* |  |

### interlok-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.12.1 *(from 10.12.0)* |  |
|  | com.solacesystems:sol-jcsmp:10.12.1 *(from 10.12.0)* |  |
|  | com.solacesystems:sol-jms:10.12.1 *(from 10.12.0)* |  |

### interlok-sshtunnel ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.1.69 *(from 0.1.65)* |  |

### interlok-swift ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.prowidesoftware:pw-swift-core:SRU2020-9.1.8 *(from SRU2020-9.1.6)* |  |

### interlok-vcs-git ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.1.69 *(from 0.1.64)* |  |
|  | org.eclipse.jgit:org.eclipse.jgit.ssh.jsch:5.13.0.202109080827-r *(from 5.12.0.202106070339-r)* |  |
|  | org.eclipse.jgit:org.eclipse.jgit:5.13.0.202109080827-r *(from 5.12.0.202106070339-r)* |  |

### interlok-webservice-cxf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.cxf:cxf-rt-frontend-jaxws:3.4.5 *(from 3.4.4)* |  |
|  | org.apache.cxf:cxf-rt-transports-http:3.4.5 *(from 3.4.4)* |  |

### interlok-xa-atomikos ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.awaitility:awaitility:4.1.1 *(from 4.1.0)* |  |

### interlok-xa-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.12.1 *(from 10.12.0)* |  |
|  | com.solacesystems:sol-jcsmp:10.12.1 *(from 10.12.0)* |  |
|  | com.solacesystems:sol-jms:10.12.1 *(from 10.12.0)* |  |

### interlok-xa-wmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.2.3.0 *(from 9.1.5.0)* |  |
