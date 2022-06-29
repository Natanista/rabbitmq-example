
# RabbitMQ Pub-Sub example

Simple app for pratice RabbitMQ architecture. With this application, you can publish a message in rabbitMQ exchange through an endpoint. Project "rabbitmq-consumer" reads the message queue and print data to you in the console
## Run Locally

Run this command to start rabbitMQ in a docker container on port 15672
```bash
docker run -d --hostname my-rabbit --name some-rabbit -p 15672:15672 -p 5672:5672 rabbitmq:3-management```
```


Clone this project to yout computer 
```bash 
git clone https://github.com/Natanista/rabbitmq-example.git
```

Open the project with your favorite IDE and start it.




## API Reference

#### Post a message to queue
```PORT
 localhost:9000
```

```http
  POST /api/v1/messages
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `message` | `string` | **Required**. Message content |



## Tech Stack


**Server:** RabbitMQ, Spring Boot 

