# kafkademo
sudo bin/kafka-server-start.sh config/server-2.properties &
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic kafkatest
bin/kafka-topics.sh --list --zookeeper localhost:2181
