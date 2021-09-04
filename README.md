# go-kafka-queue-example

### Prerequisites

- Docker should be up and running in your machine
- Basic knowledge on kafka

### Steps to be followed to test

1.  Run the command to compose the docker
    `./scripts/start-kafka.sh`
2.  Run the command to install the go dependency
    `go get github.com/segmentio/kafka-go`
3.  Run the the command to create the topic
    `./scripts/create-topic.sh`
4.  Run the the command to start the producer
    `go run ./producer/producer.go`
5.  Run the the command to start the consumer
    `go run ./consumer/consumer.go`
6.  Run the the command to add messages via terminal
    `./scripts/push-topic-messages.sh`
7.  Run the the command to view the messages of the topic in terminal
    `./scripts/view-topic-messages.sh`
