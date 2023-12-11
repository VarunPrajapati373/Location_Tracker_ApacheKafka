# Location Tracker System Using APACHE KAFKA

Here we have used Apache kafka tool for getting live tracking of a person based on its longitude and latitude.

## How to run this application

1. Download the zip from here and setup the code in your STS.
2. Download Apache Kafka from the kafka site.
3. user the below command to run the server of Apache.

## Commands

```
1. unzip the downloaded kafka file - $ tar -xzf kafka_2.13-3.6.1.tgz
2. Before starting Kafka server you need to start ZooKeeper - $ bin/zookeeper-server-start.sh config/zookeeper.properties
3. open another terminal session and run - $ bin/kafka-server-start.sh config/server.properties
4. create topic and events into topic - $ bin/kafka-console-producer.sh --topic quickstart-events --bootstrap-server localhost:9092
                                         > This is my first event
                                         >  This is my second event
5. Read events from consumer - $ bin/kafka-console-consumer.sh --topic quickstart-events --from-beginning --bootstrap-server localhost:9092
