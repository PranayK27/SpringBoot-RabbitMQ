http://localhost:8080/api/v1/publish?message=sample_message

http://localhost:8080/api/v1/publish --> raw --> json
{
"id": 1,
"firstName": "Pranay",
"lastName": "Kekre"
}

RabbitMQ is a message queue software (message broker/queue manager) that acts as an intermediary platform where different applications can send and receive messages.

We will use the Spring AMQP module to work with RabbitMQ in the Spring boot application as AMQP messaging solutions.

Spring Boot RabbitMQ Architecture with Multiple Queues
The Producer is an application that sends messages to the RabbitMQ broker and the Consumer is an application that reads messages from the RabbitMQ broker.

In this tutorial, we will implement below Spring Boot RabbitMQ architecture flow:

Spring Boot RabbitMQ Multiple Queues Example
We will create two Queues:
1.pranay
2.pranay_json

In the "pranay" queue, we will store messages of the type String.

In the "pranay_json" queue, we will store messages of the type JSON.

Prerequisites
Docker - Install and set up RabbitMQ locally as a Docker container using Docker.