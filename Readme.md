

Create a new topic
```
kafka-topics --bootstrap-server localhost:9092 --topic first_topic --create --partitions 3 --replication-factor 1
```

Consumer read from topic
```
kafka-console-consumer --bootstrap-server localhost:9092 --topic to-process --formatter kafka.tools.DefaultMessageFormatter --property print.timestamp=true --property print.key=true --property print.value=true
```



### Helpful resoursces

1. [Kafka consumer CLI](https://www.conduktor.io/kafka/kafka-consumer-cli-tutorial)
