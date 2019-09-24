# Enhance Openshift container platform
Add more to the Openshift platform to take your systems to the next level of operability and visibility

## Prereuisite
- RedHat Openshift Container platform. The below is tested on OKD and Openshift 3.10, 3.11

## Distributed Logging
Openshift has built-in centralized logging using Elasticsearch Fluentd and Kibana (EFK). This EFK stack uses older versions of Elastic and Kibana with no alerting and security features. OpenDistro Elasticsearch provides free alerting, monitoring and security features and can be installed on a commodity hardware outside of Openshift platform. [Read more...](openshift/efk/README.md)

## Distributed messaging
- Use [Strimzi Kafka](https://strimzi.io/) that is a Kubernetes compliant version of Apache Kafka. [Read more...](openshift/kafka/README.md)
- Use Kafka Manager to manage Kafka brokers, topics, partitions. [Read more...](openshift/kafka-manager/README.md)

## Distributed coordination
Apache Zookeeper is the distributed coordination component that is used by Apache Kafka, Apache Storm, Apache Nifi, Apache Hadoop and many more. Install Kubernetes compliant version with  json logging and could that can be used by business applications as well. [Read more...](openshift/zookeeper/README.md)

## Distributed flow pipeline and service mesh
Apache Nifi can be used as the glue and backbone for all microservices. Nifi provides service mesh capabilities, transformers, security, dynamic throttling. [Read more...](openshift/nifi/README.md)

## Monitoring
- Deploy Grafana to visualize metrics and set alerts. [Read more...](openshift/monitoring/grafana/README.md)
- Coming soon....Prometheus