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

> Microservices are an architectural style in which an application is composed of small, independent, and loosely coupled services that communicate with each other over a network. Each microservice is responsible for a specific piece of functionality. 

### Event-driven architecture can be beneficial in a microservices environment in the following ways:

  - Decoupling: EDA enables microservices to be loosely coupled. Services can interact with each other through events without needing to know the details of the other services. This reduces dependencies and makes it easier to change or update individual services without affecting the entire system.

- Scalability: Microservices can be independently scaled based on their event processing needs. When an event generates a significant workload, you can scale the corresponding microservice to handle it, ensuring optimal resource allocation.

- Asynchronous Communication: EDA promotes asynchronous communication between microservices. This means that services can process events independently and do not have to wait for immediate responses. This can improve system performance and responsiveness.

- Fault Tolerance: EDA can enhance fault tolerance by allowing event consumers to handle events even when certain parts of the system are temporarily unavailable. Event data can be stored in durable event logs or message queues, ensuring no data is lost.

- Event-Driven Data Flow: Microservices can use events to update their internal data stores or communicate changes to other services. This makes it easier to maintain data consistency across services.

In summary, event-driven architecture complements microservices by providing a scalable, decoupled, and resilient communication model. It helps microservices work together efficiently while allowing for independent development, scaling, and fault tolerance. This combination of architectural patterns can be especially valuable in building complex and adaptable systems.

Image describing the difference between monolithic vs micro services architecture :

![image](https://github.com/izzypt/FastAPI_Microservices/assets/73948790/22a7d1f3-ec71-4a2b-9713-56c9acb5a036)
