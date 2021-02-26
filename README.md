# Kafka Installation and Commands
## http://cloudurable.com/blog/what-is-kafka/index.html
## https://tecadmin.net/install-apache-kafka-ubuntu/
## https://dattell.com/data-architecture-blog/apache-kafka-optimization/
## https://dattell.com/data-architecture-blog/kafka-optimization-how-many-partitions-are-needed/
## https://data-flair.training/blogs/kafka-performance-tuning/
## https://www.cloudkarafka.com/blog/2018-09-12-performance-optimization-apache-kafka-brokers-cloudkarafka.html
## https://www.instaclustr.com/the-power-of-kafka-partitions-how-to-get-the-most-out-of-your-kafka-cluster/
## https://www.confluent.io/blog/how-choose-number-topics-partitions-kafka-cluster/

## Commands:
### sudo bin/kafka-server-start.sh config/server-1.properties &
### sudo bin/kafka-server-start.sh config/server-2.properties &
### bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic kafkatest
### bin/kafka-topics.sh --list --zookeeper localhost:2181
### bin/kafka-topics.sh --describe --zookeeper localhost:2181  --topic kafkatest
### bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 3 --partitions 1 --topic replicatedkafkatest
### bin/kafka-console-producer.sh --broker-list localhost:9092 --topic kafkatest
### bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic kafkatest --from-beginning
