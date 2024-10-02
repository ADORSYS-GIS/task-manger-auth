# Task Manager Auth

A comprehensive Spring Boot-based Task Management Application that supports full CRUD operations for tasks, integrated with JWT authentication and role-based authorization for secure user management. The application also features a fully interactive Swagger UI for API documentation and testing.

## Features

- **CRUD Operations**: Create, read, update, and delete tasks.
- **User Authentication & Authorization**: Secure login and registration using Spring Security and JWT tokens.
- **Role-Based Access Control**: Restrict task management operations based on user roles (Admin/User).
- **Swagger API Documentation**: Full Swagger integration to interact with and explore the API.
- **Custom Error Handling**: Manage errors with customized responses for API calls.
  
## Technologies Used

- **Java 17**
- **Spring Boot 3**
  - Spring Data JPA
  - Spring Security
  - JWT (JSON Web Token)
- **Maven**: Dependency management and build automation.
- **H2 Database**: In-memory database for development/testing purposes.
- **Swagger UI**: API documentation and testing interface.
  
## Getting Started

### Prerequisites

Before running the application, ensure you have the following installed on your machine:

- [JDK 17](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html)
- [Maven](https://maven.apache.org/install.html)
- [Git](https://git-scm.com/)

### Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/task-manager-auth.git
   cd task-manager-auth

2. **Build the application**:

   ```bash
   mvn clean install


3. **Run the application**:

   ```bash
   mvn spring-boot:run

4. **Access Swagger UI**:

   Once the application is running, visit the Swagger UI to explore and test the API endpoints:

**Swagger UI:** http://localhost:9090/swagger-ui.html
**API Documentation:** http://localhost:9090/v3/api-docs


   

# Usage
### Swagger API Documentation
The application comes with an integrated Swagger UI, allowing you to explore and test the available endpoints interactively. Visit the Swagger UI at http://localhost:9090/swagger-ui.html.

**Authentication & Authorization**
The application uses JWT tokens for authentication and authorization. Here's how the authentication flow works:

1. Register: A user can register with the /auth/register endpoint.

2. Login: Use the /auth/login endpoint to receive a JWT token.

3. Access Protected Endpoints: Use the JWT token in the Authorization header (Bearer <token>) to access protected endpoints, such as creating or managing tasks.

## Task Management
### The following operations are supported:

Create a Task: (POST) /tasks
View All Tasks: (GET) /tasks
View a Task by ID: (GET) /tasks/{id}
Update a Task: (PUT) /tasks/{id}
Delete a Task: (DELETE) /tasks/{id}
**Note: Task management endpoints are protected, and users will need a valid JWT token to perform any operations.**



