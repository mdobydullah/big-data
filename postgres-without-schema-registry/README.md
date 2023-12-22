<p align="center">
    <img src="https://cdn.shouts.dev/media/400/apache-kafka-logo.png" width="150"/>
</p>

Apache Kafka is a distributed event store and stream-processing platform. It is an open-source system developed by the Apache Software Foundation written in Java and Scala. The project aims to provide a unified, high-throughput, low-latency platform for handling real-time data feeds.

Run on Docker
--
Clone repository
```bash
git clone https://github.com/mdobydullah/kafka-cmak-docker.git
cd kafka-cmak-docker
```
Run
```bash
docker compose up -d --build
```

Move into Kafka container
```bash
docker exec -it kafka /bin/sh
```

Go to Kafka `bin` folder

```bash
cd /opt/bitnami/kafka/bin
```

Create Kafka topic
```bash
kafka-topics.sh --create --topic topicName --bootstrap-server localhost:9092
```

Start Producer app (CLI)
```bash
kafka-console-producer.sh --topic topicName --bootstrap-server localhost:9092
```

Start Consumer app (CLI)
```bash
kafka-console-consumer.sh --topic topicName --from-beginning --bootstrap-server localhost:9092
```

How Kafka Works
--
<p align="center">
    <img src="https://cdn.shouts.dev/media/399/how-kafka-works.png"/>
</p>

Kafka Streams
--
<p align="center">
    <img src="https://cdn.shouts.dev/media/401/apache-kafka-streams.jpeg"/>
</p>

CMAK
--
CMAK is a tool for managing Apache Kafka clusters.
<p align="center">
    <img src="https://cdn.shouts.dev/media/402/cmak.png"/>
</p>