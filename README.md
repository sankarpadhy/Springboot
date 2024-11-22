# Spring Boot Microservices Learning Project

This project is a hands-on learning exercise focusing on building microservices using Spring Boot, with emphasis on:
- Maven package management
- Docker containerization
- Service discovery using Netflix Eureka
- Docker Compose for multi-container orchestration

## Project Structure

```
Base/
├── eureka/                 # Eureka Server (Service Registry)
├── service1/              # Microservice 1
├── service2/              # Microservice 2
└── docker-compose.yml    # Docker Compose configuration
```

## Technologies Used

- **Spring Boot**: Framework for creating microservices
- **Spring Cloud Netflix Eureka**: Service discovery
- **Maven**: Dependency management and build tool
- **Docker**: Containerization
- **Docker Compose**: Container orchestration

## Learning Objectives

1. **Maven Package Management**
   - Understanding parent-child POM structure
   - Managing dependencies across multiple modules
   - Building multiple services using Maven

2. **Docker Containerization**
   - Creating Dockerfiles for Spring Boot applications
   - Building Docker images
   - Understanding container configurations

3. **Docker Compose**
   - Multi-container application setup
   - Service networking
   - Environment configuration
   - Container orchestration

4. **Service Discovery**
   - Setting up Eureka Server
   - Service registration and discovery
   - Client-side service discovery

## Getting Started

### Prerequisites
- Java 17 or later
- Maven 3.6 or later
- Docker Desktop
- Git

### Building the Application

1. Clone the repository:
   ```bash
   git clone https://github.com/sankarpadhy/Springboot.git
   ```

2. Build the services:
   ```bash
   mvn clean package -DskipTests
   ```

3. Build and start the containers:
   ```bash
   docker-compose up --build
   ```

### Accessing the Services

- Eureka Server: http://localhost:8761
- Service1: http://localhost:8081
- Service2: http://localhost:8082

## Key Concepts Learned

1. **Maven Multi-Module Project**
   - Parent POM configuration
   - Dependency management
   - Module coordination

2. **Docker Configuration**
   - Multi-stage builds
   - Layer optimization
   - Environment configuration

3. **Docker Compose Features**
   - Service definition
   - Networking
   - Dependencies
   - Port mapping

4. **Microservices Architecture**
   - Service discovery
   - Configuration management
   - Container orchestration

## Project Components

### Eureka Server
- Central service registry
- Handles service registration and discovery
- Configuration in `application.yml`

### Service1 & Service2
- Sample microservices
- Register with Eureka Server
- Demonstrate service discovery

### Docker Configuration
- Individual Dockerfiles for each service
- Docker Compose for orchestration
- Bridge network for inter-service communication

## Next Steps

Potential areas for further learning:
1. Adding Spring Cloud Config Server
2. Implementing API Gateway
3. Adding service-to-service communication
4. Implementing circuit breakers
5. Adding monitoring and logging

## Contributing

This is a learning project. Feel free to fork and experiment with different configurations and setups.

## License

This project is open-source and available under the MIT License.
