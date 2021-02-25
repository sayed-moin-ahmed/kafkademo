# Kafka Installation and Commands
## http://cloudurable.com/blog/what-is-kafka/index.html
## https://tecadmin.net/install-apache-kafka-ubuntu/

## Commands:
### sudo bin/kafka-server-start.sh config/server-1.properties &
### sudo bin/kafka-server-start.sh config/server-2.properties &
### bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic kafkatest
### bin/kafka-topics.sh --list --zookeeper localhost:2181
### bin/kafka-topics.sh --describe --zookeeper localhost:2181  --topic kafkatest
### bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 3 --partitions 1 --topic replicatedkafkatest
