# go-kafka-queue-example

### Prerequisites

- Docker should be up and running in your machine
- Basic knowledge on kafka

### Steps to be followed to test

1.  Run below command to compose the docker
    `./scripts/start-kafka.sh`
2.  Run below command to install the go dependency
    `go get github.com/segmentio/kafka-go`
3.  Run the below command to create the topic
    `./scripts/create-topic.sh`
4.  Run the below command to start the producer
    `go run ./producer/producer.go`
5.  Run the below command to start the consumer
    `go run ./consumer/consumer.go`
6.  Run the below command to add messages via terminal
    `./scripts/push-topic-messages.sh`
7.  Run the below command to view the messages of the topic in terminal
    `./scripts/view-topic-messages.sh`
