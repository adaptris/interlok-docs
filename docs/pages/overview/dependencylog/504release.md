## Version 5.0.4 ##

### bip-services ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.json:json:20241224 *(from 20240303)* |  |

### interlok-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |
|  | org.springframework:spring-beans:5.3.39 *(from 5.3.33)* |  |
|  | org.springframework:spring-context:5.3.39 *(from 5.3.33)* |  |

### interlok-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.24.0 *(from 5.21.0)* |  |
|  | io.netty:netty-buffer:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec-http:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-common:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport:4.1.116.Final *(from 4.1.112.Final)* |  |

### interlok-apache-geode ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-core: | org.jgroups:jgroups:5.4.1.Final *(from 5.3.11.Final)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.springframework:spring-web:5.3.39 *(from 5.3.37)* |  |

### interlok-apache-http5 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents.client5:httpclient5:5.4.1 *(from 5.3.1)* |  |

### interlok-artemis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |
|  | io.netty:netty-buffer:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec-http:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec-socks:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-common:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | org.apache.activemq:artemis-jms-server:2.38.0 *(from 2.37.0)* |  |
|  | org.apache.activemq:artemis-server:2.38.0 *(from 2.37.0)* |  |
|  | org.jgroups:jgroups:5.4.1.Final *(from 5.3.11.Final)* |  |

### interlok-aws-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.777 *(from 1.12.576)* |  |
| com.amazonaws:aws-java-sdk-sts: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kinesis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:amazon-kinesis-producer:0.15.12 *(from 0.15.11)* |  |
| com.amazonaws:aws-java-sdk-kinesis: | com.amazonaws:aws-java-sdk-bom:1.12.777 *(from 1.12.576)* |  |
| com.fasterxml.jackson.core:jackson-annotations: | com.charleskorn.kaml:kaml:0.67.0 *(from 0.61.0)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | com.google.protobuf:protobuf-java:4.29.2 *(from 3.25.3)* |  |
| io.netty:netty-buffer: | com.squareup.okio:okio-fakefilesystem:3.9.1 *(from 3.9.0)* |  |
| io.netty:netty-codec-http: | com.squareup.okio:okio:3.9.1 *(from 3.9.0)* |  |
| io.netty:netty-codec: | com.squareup.wire:wire-compiler:5.1.0 *(from 4.9.9)* |  |
| io.netty:netty-common: | com.squareup.wire:wire-schema:5.1.0 *(from 4.9.9)* |  |
| io.netty:netty-handler: | io.netty:netty-bom:4.1.116.Final *(from 4.1.112.Final)* |  |
| io.netty:netty-transport-native-epoll: | org.apache.kafka:kafka-clients:3.9.0 *(from 3.8.0)* |  |
| io.netty:netty-transport-native-kqueue: | org.jetbrains.kotlin:kotlin-bom:2.1.0 *(from 2.0.20)* |  |
| io.netty:netty-transport-native-unix-common: | org.json:json:20241224 *(from 20240303)* |  |
| io.netty:netty-transport: |  |  |

### interlok-aws-kinesis-sdk ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.777 *(from 1.12.576)* |  |
| com.amazonaws:aws-java-sdk-kinesis: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.777 *(from 1.12.576)* |  |
| com.amazonaws:aws-java-sdk-kms: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-s3 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.777 *(from 1.12.576)* |  |
| com.amazonaws:aws-java-sdk-s3: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sns ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.amazonaws:aws-java-sdk-bom:1.12.777 *(from 1.12.576)* |  |
| com.amazonaws:aws-java-sdk-sns: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sqs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.amazonaws:aws-java-sdk-core:1.12.777 *(from 1.12.576)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.amazonaws:aws-java-sdk-sqs:1.12.777 *(from 1.12.576)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws2-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-annotations:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.18.2 *(from 2.17.2)* |  |
|  | software.amazon.awssdk:apache-client:2.29.9 *(from 2.21.6)* |  |
|  | software.amazon.awssdk:sdk-core:2.29.9 *(from 2.21.6)* |  |
|  | software.amazon.awssdk:sts:2.29.9 *(from 2.21.6)* |  |

### interlok-aws2-kinesis-sdk ###
| Initial Dependencies |
| -------- |
| com.fasterxml.jackson.core:jackson-annotations: |
| com.fasterxml.jackson.core:jackson-core: |
| com.fasterxml.jackson.core:jackson-databind: |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |
| com.fasterxml.jackson:jackson-bom:2.18.2 |
| org.slf4j:jcl-over-slf4j:2.0.16 |
| org.slf4j:slf4j-api:2.0.16 |
| software.amazon.awssdk:bom:2.29.9 |
| software.amazon.awssdk:kinesis: |
| software.amazon.awssdk:sdk-core: |

### interlok-aws2-kms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-annotations:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.18.2 *(from 2.17.2)* |  |
|  | software.amazon.awssdk:kms:2.29.9 *(from 2.21.6)* |  |
|  | software.amazon.awssdk:sdk-core:2.29.9 *(from 2.21.6)* |  |

### interlok-aws2-s3 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-annotations:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.18.2 *(from 2.17.2)* |  |
|  | software.amazon.awssdk:s3:2.29.9 *(from 2.21.6)* |  |
|  | software.amazon.awssdk:sdk-core:2.29.9 *(from 2.21.6)* |  |

### interlok-aws2-sns ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-annotations:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.18.2 *(from 2.17.2)* |  |
|  | software.amazon.awssdk:sdk-core:2.29.9 *(from 2.21.6)* |  |
|  | software.amazon.awssdk:sns:2.29.9 *(from 2.21.6)* |  |

### interlok-aws2-sqs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-annotations:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-core:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.core:jackson-databind:2.18.2 *(from 2.17.2)* |  |
|  | com.fasterxml.jackson.dataformat:jackson-dataformat-cbor:2.18.2 *(from 2.17.2)* |  |
|  | software.amazon.awssdk:sdk-core:2.29.9 *(from 2.21.6)* |  |
|  | software.amazon.awssdk:sqs:2.29.9 *(from 2.21.6)* |  |

### interlok-azure-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.azure:azure-identity:1.14.2 *(from 1.13.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.azure:azure-storage-file-datalake:12.22.0 *(from 12.20.1)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-xml: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.datatype:jackson-datatype-jsr310: | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |
|  | com.microsoft.azure:msal4j:1.18.0 *(from 1.17.1)* |  |
|  | com.squareup.okio:okio:3.9.1 *(from 3.9.0)* |  |
|  | io.netty:netty-codec-http2:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec-http:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-resolver-dns:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.116.Final *(from 4.1.112.Final)* |  |

### interlok-azure-cosmosdb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.json:json:20241224 *(from 20240303)* |  |

### interlok-cassandra ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |
|  | io.netty:netty-codec:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.116.Final *(from 4.1.112.Final)* |  |

### interlok-cluster-manager ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jgroups:jgroups:5.4.1.Final *(from 5.3.11.Final)* |  |

### interlok-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.21 *(from 1.4.20)* |  |
|  | commons-io:commons-io:2.18.0 *(from 2.16.1)* |  |
|  | org.apache.logging.log4j:log4j-1.2-api:2.24.3 *(from 2.23.1)* |  |
|  | org.apache.logging.log4j:log4j-api:2.24.3 *(from 2.23.1)* |  |
|  | org.apache.logging.log4j:log4j-core:2.24.3 *(from 2.23.1)* |  |
|  | org.apache.logging.log4j:log4j-slf4j2-impl:2.24.3 *(from 2.23.1)* |  |
|  | org.eclipse.jetty.http2:http2-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.http2:http2-common:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.http2:http2-hpack:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.http2:http2-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.websocket:websocket-javax-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.websocket:websocket-javax-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-alpn-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-alpn-java-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-alpn-java-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-alpn-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-annotations:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-deploy:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-http:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-io:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-jaspi:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-jmx:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-jndi:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-plus:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-quickstart:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-rewrite:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-security:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-servlet:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-servlets:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-util-ajax:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-util:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-webapp:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-xml:10.0.24 *(from 10.0.23)* |  |

### interlok-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.21 *(from 0.2.19)* |  |
|  | com.thoughtworks.xstream:xstream:1.4.21 *(from 1.4.20)* |  |
|  | com.zaxxer:HikariCP:6.2.1 *(from 5.1.0)* |  |
|  | commons-io:commons-io:2.18.0 *(from 2.16.1)* |  |
|  | io.github.classgraph:classgraph:4.8.179 *(from 4.8.175)* |  |
|  | org.bouncycastle:bcmail-jdk18on:1.79 *(from 1.78.1)* |  |
|  | org.bouncycastle:bcpkix-jdk18on:1.79 *(from 1.78.1)* |  |
|  | org.bouncycastle:bcprov-jdk18on:1.79 *(from 1.78.1)* |  |
|  | org.eclipse.jetty.http2:http2-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.http2:http2-common:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.http2:http2-hpack:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.http2:http2-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.websocket:websocket-javax-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty.websocket:websocket-javax-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-alpn-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-alpn-java-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-alpn-java-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-alpn-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-annotations:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-client:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-deploy:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-http:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-io:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-jaspi:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-jmx:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-jndi:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-plus:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-quickstart:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-rewrite:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-security:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-server:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-servlet:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-servlets:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-util-ajax:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-util:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-webapp:10.0.24 *(from 10.0.23)* |  |
|  | org.eclipse.jetty:jetty-xml:10.0.24 *(from 10.0.23)* |  |
|  | org.quartz-scheduler:quartz:2.5.0 *(from 2.3.2)* |  |

### interlok-core-apt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.21 *(from 1.4.20)* |  |

### interlok-csv-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |

### interlok-csv-schema ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.scala-lang.plugins:scala-continuations-library_2.12:1.0.3 | org.scala-lang:scala-library:2.13.15 *(from 2.13.14)* | ~~org.scala-lang.plugins:scala-continuations-library_2.11:1.0.3~~ |

### interlok-elastic-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | joda-time:joda-time:2.13.0 *(from 2.12.7)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: | org.apache.commons:commons-csv:1.12.0 *(from 1.11.0)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: | org.apache.logging.log4j:log4j-api:2.24.3 *(from 2.23.1)* |  |
|  | org.apache.logging.log4j:log4j-core:2.24.3 *(from 2.23.1)* |  |
|  | org.elasticsearch:elasticsearch-x-content:7.17.26 *(from 7.17.23)* |  |
|  | org.elasticsearch:elasticsearch:7.17.26 *(from 7.17.23)* |  |

### interlok-elastic-rest ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | joda-time:joda-time:2.13.0 *(from 2.12.7)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: | org.apache.logging.log4j:log4j-api:2.24.3 *(from 2.23.1)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: | org.apache.logging.log4j:log4j-core:2.24.3 *(from 2.23.1)* |  |
|  | org.elasticsearch.client:elasticsearch-rest-client-sniffer:7.17.26 *(from 7.17.23)* |  |
|  | org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.26 *(from 7.17.23)* |  |
|  | org.elasticsearch:elasticsearch-x-content:7.17.26 *(from 7.17.23)* |  |

### interlok-elastic-sdk ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | co.elastic.clients:elasticsearch-java:7.17.26 *(from 7.17.23)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: | joda-time:joda-time:2.13.0 *(from 2.12.7)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: | org.apache.logging.log4j:log4j-api:2.24.3 *(from 2.23.1)* |  |
|  | org.apache.logging.log4j:log4j-core:2.24.3 *(from 2.23.1)* |  |
|  | org.elasticsearch.client:elasticsearch-rest-high-level-client:7.17.26 *(from 7.17.23)* |  |
|  | org.elasticsearch:elasticsearch-x-content:7.17.26 *(from 7.17.23)* |  |

### interlok-failover ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jgroups:jgroups:5.4.1.Final *(from 5.3.11.Final)* |  |

### interlok-filesystem ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.hierynomus:smbj:0.14.0 *(from 0.13.0)* |  |
|  | org.apache.tika:tika-core:3.0.0 *(from 2.9.2)* |  |
|  | org.json:json:20241224 *(from 20240303)* |  |

### interlok-gcloud-pubsub ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
|  | com.google.cloud:google-cloud-pubsub:1.135.0 *(from 1.132.1)* |  |
|  | com.google.protobuf:protobuf-java-util:4.29.2 *(from 3.25.3)* |  |
|  | com.google.protobuf:protobuf-java:4.29.2 *(from 3.25.3)* |  |
|  | io.grpc:grpc-alts:1.69.0 *(from 1.66.0)* |  |
|  | io.grpc:grpc-auth:1.69.0 *(from 1.66.0)* |  |
|  | io.grpc:grpc-context:1.69.0 *(from 1.66.0)* |  |
|  | io.grpc:grpc-googleapis:1.69.0 *(from 1.66.0)* |  |
|  | io.grpc:grpc-inprocess:1.69.0 *(from 1.66.0)* |  |
|  | io.grpc:grpc-netty:1.69.0 *(from 1.66.0)* |  |
|  | io.grpc:grpc-protobuf:1.69.0 *(from 1.66.0)* |  |
|  | io.grpc:grpc-services:1.69.0 *(from 1.66.0)* |  |
|  | io.grpc:grpc-stub:1.69.0 *(from 1.66.0)* |  |
|  | io.netty:netty-codec-http2:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec-http:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.116.Final *(from 4.1.112.Final)* |  |

### interlok-jclouds-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |

### interlok-jdbc ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |

### interlok-jms3-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.netty:netty-bom:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | org.apache.activemq:artemis-jakarta-client:2.39.0 *(from 2.37.0)* |  |

### interlok-jmx-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.21 *(from 1.4.20)* |  |
|  | commons-io:commons-io:2.18.0 *(from 2.16.1)* |  |

### interlok-jmx-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.21 *(from 1.4.20)* |  |
|  | commons-io:commons-io:2.18.0 *(from 2.16.1)* |  |
|  | io.netty:netty-buffer:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec-http:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-codec:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-common:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport:4.1.116.Final *(from 4.1.112.Final)* |  |

### interlok-jmx-jms-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.21 *(from 1.4.20)* |  |
|  | commons-io:commons-io:2.18.0 *(from 2.16.1)* |  |

### interlok-jmx-jms-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.thoughtworks.xstream:xstream:1.4.21 *(from 1.4.20)* |  |
|  | commons-io:commons-io:2.18.0 *(from 2.16.1)* |  |
|  | org.junit.jupiter:junit-jupiter-engine:5.11.4 *(from 5.11.0)* |  |

### interlok-jmx-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.25.1 *(from 10.24.1)* |  |
|  | com.solacesystems:sol-jcsmp:10.25.1 *(from 10.24.1)* |  |
|  | com.solacesystems:sol-jms:10.25.1 *(from 10.24.1)* |  |
|  | com.thoughtworks.xstream:xstream:1.4.21 *(from 1.4.20)* |  |
|  | commons-io:commons-io:2.18.0 *(from 2.16.1)* |  |

### interlok-jq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.auth0:jwks-rsa:0.22.1 | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | net.thisptr:jackson-jq-extra:1.0.1 *(from 1.0.0-preview.20240207)* |  |
|  | net.thisptr:jackson-jq:1.0.1 *(from 1.0.0-preview.20240207)* |  |

### interlok-jruby ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jruby:jruby:9.4.9.0 *(from 9.4.8.0)* |  |

### interlok-jslt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.auth0:jwks-rsa:0.22.1 | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.auth0:jwks-rsa:0.22.1 | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-annotations: | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |
| com.fasterxml.jackson.core:jackson-core: | org.json:json:20241224 *(from 20240303)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-json-streaming ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.auth0:jwks-rsa:0.22.1 | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-json-web-token ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.auth0:jwks-rsa:0.22.1 | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.bouncycastle:bcpg-jdk18on:1.79 *(from 1.78.1)* |  |
|  | org.bouncycastle:bcprov-jdk18on:1.79 *(from 1.78.1)* |  |
|  | org.json:json:20241224 *(from 20240303)* |  |

### interlok-kafka ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | ch.qos.logback:logback-classic:1.5.16 *(from 1.5.7)* |  |
|  | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
|  | io.netty:netty-codec:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-handler:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | org.apache.kafka:kafka-clients:3.9.0 *(from 3.8.0)* |  |
|  | org.apache.kafka:kafka_2.13:3.9.0 *(from 3.8.0)* |  |
|  | org.apache.zookeeper:zookeeper:3.9.3 *(from 3.9.2)* |  |

### interlok-kie ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.21 *(from 1.4.20)* |  |

### interlok-logging ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.logging.log4j:log4j-api:2.24.3 *(from 2.23.1)* |  |
|  | org.apache.logging.log4j:log4j-core:2.24.3 *(from 2.23.1)* |  |

### interlok-mongodb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |

### interlok-mqtt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | commons-codec:commons-codec:1.17.2 *(from 1.17.1)* |  |

### interlok-nats ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.nats:jnats:2.20.5 *(from 2.20.2)* |  |

### interlok-oauth-azure ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.nimbusds:nimbus-jose-jwt:9.47 *(from 9.40)* |  |

### interlok-oauth-gcloud ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-core:2.18.2 *(from 2.17.2)* |  |
|  | com.google.auth:google-auth-library-oauth2-http:1.30.1 *(from 1.24.1)* |  |
|  | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |
|  | io.grpc:grpc-context:1.69.0 *(from 1.66.0)* |  |

### interlok-oauth-generic ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |

### interlok-oauth-salesforce ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |

### interlok-okhttp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.squareup.okio:okio:3.9.1 *(from 3.9.0)* |  |

### interlok-pdf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.google.guava:guava:33.4.0-jre *(from 33.3.0-jre)* |  |
|  | commons-io:commons-io:2.18.0 *(from 2.16.1)* |  |
|  | org.apache.xmlgraphics:batik-extension:1.18 *(from 1.17)* |  |
|  | org.apache.xmlgraphics:batik-transcoder:1.18 *(from 1.17)* |  |
|  | org.apache.xmlgraphics:fop:2.10 *(from 2.9)* |  |

### interlok-pgp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.bouncycastle:bcpg-jdk18on:1.79 *(from 1.78.1)* |  |
|  | org.bouncycastle:bcprov-jdk18on:1.79 *(from 1.78.1)* |  |

### interlok-proxy ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.httpcomponents.client5:httpclient5:5.4.1 *(from 5.3.1)* |  |

### interlok-rabbitmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.rabbitmq:amqp-client:5.24.0 *(from 5.21.0)* |  |

### interlok-rest-metrics-jvm ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-core:1.13.7 *(from 1.13.3)* |  |

### interlok-rest-provider-datadog ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | io.micrometer:micrometer-registry-datadog:1.13.7 *(from 1.13.3)* |  |

### interlok-rest-provider-prometheus ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| io.micrometer:micrometer-registry-prometheus:1.13.7 |  | ~~io.micrometer:micrometer-registry-prometheus-simpleclient:1.13.3~~ |

### interlok-scripting ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.graalvm.js:js-scriptengine:23.0.7 *(from 23.0.5)* |  |
|  | org.graalvm.js:js:23.0.7 *(from 23.0.5)* |  |
|  | org.graalvm.sdk:graal-sdk:23.0.7 *(from 23.0.5)* |  |

### interlok-service-tester ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | commons-io:commons-io:2.18.0 *(from 2.16.1)* |  |

### interlok-service-tester-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-databind: | org.json:json:20241224 *(from 20240303)* |  |

### interlok-service-tester-wiremock ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.18.2 *(from 2.17.2)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.nimbusds:nimbus-jose-jwt:9.47 *(from 9.40)* |  |
| com.fasterxml.jackson.core:jackson-databind: | io.netty:netty-bom:4.1.116.Final *(from 4.1.112.Final)* |  |
|  | io.swagger.parser.v3:swagger-parser:2.1.24 *(from 2.1.22)* |  |
|  | org.mozilla:rhino:1.8.0 *(from 1.7.15)* |  |

### interlok-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.25.1 *(from 10.24.1)* |  |
|  | com.solacesystems:sol-jcsmp:10.25.1 *(from 10.24.1)* |  |
|  | com.solacesystems:sol-jms:10.25.1 *(from 10.24.1)* |  |

### interlok-sshtunnel ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.21 *(from 0.2.19)* |  |

### interlok-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.junit.jupiter:junit-jupiter-api:5.11.4 *(from 5.11.0)* |  |
|  | org.junit.jupiter:junit-jupiter-engine:5.11.4 *(from 5.11.0)* |  |

### interlok-vcs-git ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.21 *(from 0.2.19)* |  |

### interlok-webspheremq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.4.1.1 *(from 9.3.5.1)* |  |
|  | org.json:json:20241224 *(from 20240303)* |  |

### interlok-xa-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.solacesystems:sol-common:10.25.1 *(from 10.24.1)* |  |
|  | com.solacesystems:sol-jcsmp:10.25.1 *(from 10.24.1)* |  |
|  | com.solacesystems:sol-jms:10.25.1 *(from 10.24.1)* |  |

### interlok-xa-wmq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.ibm.mq:com.ibm.mq.allclient:9.4.1.1 *(from 9.3.5.1)* |  |
|  | org.json:json:20241224 *(from 20240303)* |  |
