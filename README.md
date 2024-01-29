
# property server management application api

A brief description of what this project does and who it's for


## Features

- User registration and login with JWT authentication
- Password encryption using BCrypt

## Technologies

- Spring Boot 3.0
- Spring Security
- JSON Web Tokens (JWT)
- BCrypt
- Maven




## Getting Started
To get started with this project, you will need to have the following installed on your local machine:

- JDK 17+
- Maven 3+
## Installation

To build and run the project, follow these steps:

Clone the repository:

```bash
git clone https://github.com/orsa-io/orsa-salon-server.git
``` 

Navigate to the project directory: 

```bash
cd orsa-salon-server
``` 

Run docker compose to use Postgres:
```bash
docker-compose up --build
```

Build the project:

```bash
mvn clean install
```

Run the project: 
```bash
mvn spring-boot:run
```

-> The application will be available at http://localhost:8082.

    
## API Reference

#### Login

```http
  POST /api/v1/accounts/login
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `email` | `string` | **Required**. Body parameter |
| `password` | `string` | **Required**. Body parameter |
