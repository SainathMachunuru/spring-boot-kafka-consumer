# spring-boot-kafka-consumer

Spring Boot with Kafka Consumer Example

This Project covers how to use Spring Boot with Spring Kafka to Consume JSON/String message from Kafka topics

Start Zookeeper

bin/zookeeper-server-start.sh config/zookeeper.properties

Start Kafka Server

bin/kafka-server-start.sh config/server.properties

Create Kafka Topic

bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example

bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example_json

Publish to the Kafka Topic via Console

bin/kafka-console-producer.sh --broker-list localhost:9092 --topic Kafka_Example

bin/kafka-console-producer.sh --broker-list localhost:9092 --topic Kafka_Example_json

kafka windows commands:

zookeeper-server-start.bat ../../config/zookeeper.properties

kafka-server-start.bat ../../config/server.properties

kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example

kafka-console-producer.bat --broker-list localhost:9092 --topic Kafka_Example
