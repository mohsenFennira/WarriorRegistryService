# WarriorRegistryService
# Eureka Service Registry

This repository contains a basic implementation of a **Service Registry** using **Spring Cloud Eureka**. It acts as a discovery server for registering microservices, enabling them to discover and communicate with each other.

## Features

- **Service Discovery:** Microservices can register themselves with the Eureka server.
- **Instance Management:** Track registered services and manage service instances.
- **Client-Side Load Balancing:** Eureka helps in client-side load balancing by distributing the traffic between service instances.

## Prerequisites

- **Java 23** installed.
- **Maven** installed.
- **Spring Boot** and **Spring Cloud Netflix Eureka** dependencies.


1. Build and run the application:

    ```bash
    mvn clean install
    mvn spring-boot:run
    ```

2. The Eureka dashboard will be available at:

    ```
    http://localhost:8761
    ```

## Configuration

Eureka Server configuration can be adjusted in the `application.properties` or `application.yml` file. Below is an example for `application.properties`:

```properties
server.port=8761
eureka.client.register-with-eureka=false
eureka.client.fetch-registry=false
