# kafka-prod

refer to bitnami, to create prod kafka:

> helm install -n kafka --set replicaCount=3,zookeeper.replicaCount=3,defaultReplicationFactor=3,offsetsTopicReplicationFactor=3,transactionStateLogReplicationFactor=3,transactionStateLogMinIsr=3,externalAccess.enabled=true,externalAccess.service.type=NodePort,metrics.kafka.enabled=true,metrics.jmx.enabled=true,zookeeper.metrics.enabled=true,externalAccess.service.nodePorts[0]=30100,externalAccess.service.nodePorts[1]=30101,externalAccess.service.nodePorts[2]=30102,externalAccess.service.domain=192.168.1.212 kafka bitnami/kafka

