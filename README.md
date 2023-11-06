# FastAPI_Microservices
- A simple Microservices app using Python FastAPI with React on the frontend.  
- RedisJSON as a Database and dispatch events with Redis Streams.
- RedisJSON is a NoSQL database just like MongoDB and Redis Streams is an Event Bus just like RabbitMQ.

![image](https://github.com/izzypt/FastAPI_Microservices/assets/73948790/30c59cda-78d5-4164-8ced-2edc77a12f35)

### What we will build

A simple microservices app using FastAPI and React.

We will have 2 main microservices:
- Inventory -> Will store the products
- Payments -> Will purchase the products

The data will be stored in RedisJSON, which is a database similar to MongoBD.

We will send events from one microservice to another using Redis streams.

# Some concepts about Event-driven architecture (EDA)  and micro services

  ### Events: 
  Events are the core of EDA (Event Driven Architecture ). 
  They represent messages or notifications about things that have happened in the system. Events can carry information about the event itself, such as its type, timestamp, and relevant data.

  ### Event Producers: 
  Event producers are responsible for generating and emitting events. These can be various components in a system, such as applications, services, sensors, or users.

  ### Event Consumers: 
  Event consumers are components or services that subscribe to specific events and react to them. They process events by executing predefined actions or event handlers.

  ### Event Bus or Message Broker: 
  An event bus or message broker is a central component that acts as an intermediary for events. It allows event producers to publish events and event consumers to subscribe to and receive events. Popular technologies like Apache Kafka, RabbitMQ, and Amazon SNS/SQS are often used as event buses.
