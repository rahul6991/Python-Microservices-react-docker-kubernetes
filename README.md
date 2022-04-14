# Python-Microservices-react-docker-kubernetes
This project is for getting a industry level system design experience in microservices in python

Provided DOcker file for kafka and zooker:
- install Docker
- run command
  - download docker image: docker pull bitnami/kafka
  - download zooker image: docker pull wurstmeister/zookeeper
- change directory to docker_kafka cd ./docker_kafka_setuo
  - run command
  - docker compose -f docker-compose.yml up -d

run CMD to create a topic 
kafka-topics --create --topic email-topic --bootstrap-server localhost:9092 --replication-factor 1 --partitions 4
