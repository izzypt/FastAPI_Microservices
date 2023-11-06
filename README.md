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

The data will be stored in RedisJSON, which is a database similar to MOngoBD.

We will send event from one microservice to another using Redis streams.
