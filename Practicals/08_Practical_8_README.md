# Practical 8 — Spring Boot Transactional Microservice

## Requirements
- Java 17+
- Maven
- PostgreSQL
- `bookflow_db`

## Configure PostgreSQL

Open:

`src/main/resources/application.yml`

Set the PostgreSQL username and password to your local values.

## Run

From this folder:

```bash
mvn spring-boot:run
```

The service runs on:

`http://localhost:8080`

Endpoints:
- `POST /orders`
- `GET /inventory/{bookId}`

The service checks available stock before creating a BORROWED order.
