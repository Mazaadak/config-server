# Config Server
## Overview
- The Config Server provides centralized configuration management for all microservices in the Mazadak platform using Spring Cloud Config.

- It exposes configuration properties from the configs repository, supports environment-specific configurations, and enables dynamic configuration updates without service restarts.

- The Config Server is the central source of truth for application configuration across the platform.

- You can find/update the config files of the platform at the [mazada-configs repo](https://github.com/Mazaadak/mazadak-configs)

## API Endpoints
- Configuration available at `http://localhost:18071/{service-name}/{profile}` when running locally
- Actuator endpoints available for health checks and monitoring 

## How to Run
You can run it via [Docker Compose](https://github.com/Mazaadak/mazadak-infrastructure) <!-- or [Kubernetes](https://github.com/Mazaadak/mazadak-k8s/) -->

## Tech Stack
- **Spring Boot 3.5.6** (Java 21)
- **Spring Cloud Config Server** - Centralized Configuration Management
- **Git** - Configuration Storage Backend
- **Netflix Eureka** - Service Discovery
- **Docker & Kubernetes** - Deployment & Containerization

## For Further Information
Refer to [Config Server Wiki Page](https://github.com/Mazaadak/.github/wiki/Config-Server).
