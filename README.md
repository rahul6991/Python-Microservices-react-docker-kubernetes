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
  
Now open up a kafka terminal and create your first kafka topic
- run command
  - docker exec -it kafka /bin/sh
    - cd /opt/kafka_2.13-2.8.1/bin
    - kafka-topics.sh --create --zookeeper zookeeper:2181 --replication-factor 1 --partitions 1 --topic email
    - kafka-topics.sh --list --zookeeper zookeeper:2181 #list all kafka topic

run CMD to create a topic 
kafka-topics --create --topic email-topic --bootstrap-server localhost:9092 --replication-factor 1 --partitions 4
