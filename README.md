# Aspnet Microservices
![microservices](https://user-images.githubusercontent.com/103562305/165698551-a321a5df-2345-4eb2-912f-f7b1213b9cf8.png)

## Whats Including In This Repository
We have implemented below **features over the run-aspnetcore-microservices repository**.

#### Catalog microservice which includes; 
* ASP.NET Core Web API application 
* REST API principles, CRUD operations
* **MongoDB database** connection and containerization
* Repository Pattern Implementation
* Swagger Open API implementation	

#### Basket microservice which includes;
* ASP.NET Web API application
* REST API principles, CRUD operations
* **Redis database** connection and containerization
* Consume Discount **Grpc Service** for inter-service sync communication to calculate product final price
* Publish BasketCheckout Queue with using **MassTransit and RabbitMQ**
  
#### Discount microservice which includes;
* ASP.NET **Grpc Server** application
* Build a Highly Performant **inter-service gRPC Communication** with Basket Microservice
* Exposing Grpc Services with creating **Protobuf messages**
* Using **Dapper for micro-orm implementation** to simplify data access and ensure high performance
* **PostgreSQL database** connection and containerization

#### Microservices Communication
* Sync inter-service **gRPC Communication**
* Async Microservices Communication with **RabbitMQ Message-Broker Service**
* Using **RabbitMQ Publish/Subscribe Topic** Exchange Model
* Using **MassTransit** for abstraction over RabbitMQ Message-Broker system
* Publishing BasketCheckout event queue from Basket microservices and Subscribing this event from Ordering microservices	
* Create **RabbitMQ EventBus.Messages library** and add references Microservices

#### Ordering Microservice
* Implementing **DDD, CQRS, and Clean Architecture** with using Best Practices
* Developing **CQRS with using MediatR, FluentValidation and AutoMapper packages**
* Consuming **RabbitMQ** BasketCheckout event queue with using **MassTransit-RabbitMQ** Configuration
* **SqlServer database** connection and containerization
* Using **Entity Framework Core ORM** and auto migrate to SqlServer when application startup
	
#### API Gateway Ocelot Microservice
* Implement **API Gateways with Ocelot**
* Sample microservices/containers to reroute through the API Gateways
* Run multiple different **API Gateway/BFF** container types	
* The Gateway aggregation pattern in Shopping.Aggregator

#### WebUI ShoppingApp Microservice
* ASP.NET Core Web Application with Bootstrap 4 and Razor template
* Call **Ocelot APIs with HttpClientFactory** and **Polly**

#### Microservices Cross-Cutting Implementations
* Implementing **Centralized Distributed Logging with Elastic Stack (ELK); Elasticsearch, Logstash, Kibana and SeriLog** for Microservices
* Use the **HealthChecks** feature in back-end ASP.NET microservices
* Using **Watchdog** in separate service that can watch health and load across services, and report health about the microservices by querying with the HealthChecks

#### Microservices Resilience Implementations
* Making Microservices more **resilient Use IHttpClientFactory** to implement resilient HTTP requests
* Implement **Retry and Circuit Breaker patterns** with exponential backoff with IHttpClientFactory and **Polly policies**

#### Ancillary Containers
* Use **Portainer** for Container lightweight management UI which allows you to easily manage your different Docker environments
* **pgAdmin PostgreSQL Tools** feature rich Open Source administration and development platform for PostgreSQL

#### Docker Compose establishment with all microservices on docker;
* Containerization of microservices
* Containerization of databases
* Override Environment variables

![81381837-08226000-9116-11ea-9489-82645b8dbfc4](https://user-images.githubusercontent.com/103562305/170031433-8d5db2dc-75fd-42a7-998c-d9ce2cec2e38.png)
