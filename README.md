# ShiftSync — Spring Cloud Config Server

**Student Name:** Chamith Bhanuka Widanapathirana  
**Student ID / Number:** 241711051  
**Slack Handle:** Chamith Bhanuka  
**GCP Project ID:** project-a58ee7a4-4913-4af2-a6d  
**Course:** ITS 2130 — Enterprise Cloud Architecture  

---

## Description

Centralized configuration management server for the ShiftSync microservices platform built with Spring Cloud Config Server. Provides centralized external configuration across environments (local development, GCP Compute Engine Managed Instance Groups) for all microservices and infrastructure components.

---

## Key Responsibilities

- **Centralized Configuration Management**: Serves configuration YAML files (`application.yml`, `scheduling-service.yml`, `notification-service.yml`, `credential-service.yml`, `api-gateway.yml`) via native / Git backends.
- **Internal Load Balancing**: Deployed behind Google Cloud Internal Load Balancer `lb-platform-config-server` on `10.0.0.10:8888` / `10.148.0.13:8888`.
- **Dynamic Refresh**: Allows microservices to fetch updated database credentials, Atlas URIs, and service discovery parameters without redeploying code.

---

## Technology Stack

- Java 25
- Spring Boot 3.x
- Spring Cloud Config Server
- Spring Boot Actuator
