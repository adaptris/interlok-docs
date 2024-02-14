## Version 4.7.0 ##

### interlok-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.0 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| org.apache.qpid:qpid-java-build:6.0.3 | io.netty:netty-buffer:4.1.87.Final *(from 4.1.84.Final)* | ~~org.apache.qpid:proton-jms:0.12.2~~ |
|  | io.netty:netty-codec-http:4.1.87.Final *(from 4.1.84.Final)* | ~~org.apache.qpid:qpid-amqp-1-0-client-jms:0.32~~ |
|  | io.netty:netty-codec:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-common:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-handler:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | org.apache.qpid:qpid-jms-client:2.1.0 *(from 1.6.0)* |  |

### interlok-apache-geode ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-artemis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| io.netty:netty-codec-socks:4.1.87.Final | io.netty:netty-buffer:4.1.87.Final *(from 4.1.84.Final)* |  |
| io.netty:netty-handler-proxy:4.1.87.Final | io.netty:netty-codec-http:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-codec:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-common:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-handler:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport:4.1.87.Final *(from 4.1.84.Final)* |  |

### interlok-aws-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.amazonaws:aws-java-sdk-sts: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kinesis ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.amazonaws:aws-java-sdk-kinesis: | com.squareup.wire:wire-compiler:4.4.3 *(from 4.4.2)* |  |
| com.fasterxml.jackson.core:jackson-annotations: | com.squareup.wire:wire-schema:4.4.3 *(from 4.4.2)* |  |
| com.fasterxml.jackson.core:jackson-core: | io.netty:netty-bom:4.1.87.Final *(from 4.1.84.Final)* |  |
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
| com.amazonaws:aws-java-sdk-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.amazonaws:aws-java-sdk-kinesis: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-kms ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.amazonaws:aws-java-sdk-kms: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-s3 ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.amazonaws:aws-java-sdk-s3: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sns ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.amazonaws:aws-java-sdk-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.amazonaws:aws-java-sdk-sns: |  |  |
| com.fasterxml.jackson.core:jackson-annotations: |  |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-aws-sqs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-core: | org.apache.httpcomponents:httpclient:4.5.14 *(from 4.5.13)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |

### interlok-azure-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-databind: | io.netty:netty-codec-http2:4.1.87.Final *(from 4.1.84.Final)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-xml: | io.netty:netty-codec-http:4.1.87.Final *(from 4.1.84.Final)* |  |
| com.fasterxml.jackson.datatype:jackson-datatype-jsr310: | io.netty:netty-codec:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-handler:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-resolver-dns:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.87.Final *(from 4.1.84.Final)* |  |

### interlok-azure-cosmosdb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-cassandra ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-databind: | io.netty:netty-codec:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-handler:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.87.Final *(from 4.1.84.Final)* |  |

### interlok-client ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.6 *(from 2.0.3)* |  |

### interlok-client-jmx ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:slf4j-api:2.0.6 *(from 2.0.3)* |  |

### interlok-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.20 *(from 1.4.19)* |  |
|  | commons-net:commons-net:3.9.0 *(from 3.8.0)* |  |
|  | org.slf4j:jcl-over-slf4j:2.0.6 *(from 2.0.3)* |  |
|  | org.slf4j:jul-to-slf4j:2.0.6 *(from 2.0.3)* |  |
|  | org.slf4j:slf4j-api:2.0.6 *(from 2.0.3)* |  |

### interlok-core ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.github.mwiede:jsch:0.2.5 *(from 0.2.4)* |  |
|  | com.thoughtworks.xstream:xstream:1.4.20 *(from 1.4.19)* |  |
|  | commons-net:commons-net:3.9.0 *(from 3.8.0)* |  |
|  | org.codehaus.jettison:jettison:1.5.3 *(from 1.2)* |  |
|  | org.slf4j:slf4j-api:2.0.6 *(from 2.0.3)* |  |

### interlok-core-apt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.20 *(from 1.4.19)* |  |

### interlok-csv-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |

### interlok-elastic-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: | org.apache.lucene:lucene-core:9.4.2 *(from 8.11.1)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-elastic-rest ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-elastic-sdk ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-cbor: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-smile: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-gcloud-pubsub ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
|  | com.google.cloud:google-cloud-pubsub:1.121.1 *(from 1.120.20)* |  |
|  | io.netty:netty-codec-http2:4.1.87.Final *(from 4.1.82.Final)* |  |
|  | io.netty:netty-codec-http:4.1.87.Final *(from 4.1.82.Final)* |  |
|  | io.netty:netty-codec:4.1.87.Final *(from 4.1.82.Final)* |  |
|  | io.netty:netty-handler-proxy:4.1.87.Final *(from 4.1.82.Final)* |  |
|  | io.netty:netty-handler:4.1.87.Final *(from 4.1.82.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.87.Final *(from 4.1.82.Final)* |  |

### interlok-jmx-activemq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.20 *(from 1.4.19)* |  |

### interlok-jmx-amqp ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.20 *(from 1.4.19)* |  |
|  | io.netty:netty-buffer:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-codec-http:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-codec:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-common:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-handler:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-kqueue:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-unix-common:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport:4.1.87.Final *(from 4.1.84.Final)* |  |

### interlok-jmx-jms-common ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.20 *(from 1.4.19)* |  |

### interlok-jmx-jms-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-core: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-databind: | com.thoughtworks.xstream:xstream:1.4.20 *(from 1.4.19)* |  |

### interlok-jmx-solace ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.20 *(from 1.4.19)* |  |

### interlok-jq ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |

### interlok-jruby ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.jruby:jruby:9.4.0.0 *(from 9.3.8.0)* |  |

### interlok-jslt ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |

### interlok-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |
| com.fasterxml.jackson.dataformat:jackson-dataformat-yaml: |  |  |

### interlok-json-streaming ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-core: |  |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-json-web-token ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |

### interlok-kafka ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
|  | io.netty:netty-codec:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-handler:4.1.87.Final *(from 4.1.84.Final)* |  |
|  | io.netty:netty-transport-native-epoll:4.1.87.Final *(from 4.1.84.Final)* |  |

### interlok-kie ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.thoughtworks.xstream:xstream:1.4.20 *(from 1.4.19)* |  |

### interlok-mongodb ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |

### interlok-oauth-gcloud ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | com.fasterxml.jackson.core:jackson-core:2.14.1 *(from 2.13.4)* |  |

### interlok-oauth-generic ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |

### interlok-oauth-salesforce ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-databind: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |

### interlok-pdf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | net.sf.cssbox:pdf2dom:2.0.3 *(from 2.0.1)* |  |
|  | org.apache.xmlgraphics:batik-extension:1.16 *(from 1.15)* |  |
|  | org.apache.xmlgraphics:batik-transcoder:1.16 *(from 1.15)* |  |

### interlok-service-tester-json ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-service-tester-wiremock ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
| com.fasterxml.jackson.core:jackson-annotations: | com.fasterxml.jackson:jackson-bom:2.14.1 *(from 2.13.4.20221013)* |  |
| com.fasterxml.jackson.core:jackson-core: | com.github.tomakehurst:wiremock-jre8:2.35.0 *(from 2.34.0)* |  |
| com.fasterxml.jackson.core:jackson-databind: |  |  |

### interlok-stubs ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.slf4j:jcl-over-slf4j:2.0.6 *(from 2.0.3)* |  |
|  | org.slf4j:slf4j-api:2.0.6 *(from 2.0.3)* |  |

### interlok-webservice-cxf ###
| New Dependencies | Updated Dependencies | Removed Dependencies |
| -------- | -------- | -------- |
|  | org.apache.cxf:cxf-rt-frontend-jaxws:3.5.5 *(from 3.5.4)* |  |
|  | org.apache.cxf:cxf-rt-transports-http:3.5.5 *(from 3.5.4)* |  |
