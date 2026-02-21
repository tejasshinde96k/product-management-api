# product-management-api
product-management-api/
<br>
├── src/main/java/com/example/productapi/
│   ├── config/
│   ├── controller/
│   ├── service/
│   ├── service/impl/
│   ├── repository/
│   ├── entity/
│   ├── dto/
│   ├── security/
│   ├── exception/
│   └── ProductApiApplication.java
│
├── src/test/java/
│
├── Dockerfile
├── docker-compose.yml
├── pom.xml
└── README.md


# Product Management REST API

Java Backend Developer Technical Assignment - Zest India

## 🚀 Tech Stack

- Java 17
- Spring Boot 3
- Spring Data JPA (Hibernate)
- PostgreSQL
- Spring Security (JWT + Refresh Token)
- Swagger / OpenAPI
- Docker & Docker Compose
- JUnit 5 & Mockito
- H2 (Testing)

---

## 📌 Architecture Overview

This project follows a layered clean architecture:

Controller Layer → Handles HTTP requests  
Service Layer → Business logic  
Repository Layer → Database interaction  
Security Layer → JWT authentication & authorization  
Exception Layer → Global error handling  

The application follows RESTful API design with versioning:

`/api/v1/products`

---

## 🔐 Security Implementation

- JWT authentication
- Refresh token rotation
- Role-based access control
- Password encryption using BCrypt
- CORS configuration
- HTTPS ready

---

## 📦 Database Design

### Product Table
- id
- product_name
- created_by
- created_on
- modified_by
- modified_on

### Item Table
- id
- product_id
- quantity

---

## 📘 API Endpoints

GET /api/v1/products  
GET /api/v1/products/{id}  
POST /api/v1/products  
PUT /api/v1/products/{id}  
DELETE /api/v1/products/{id}  
GET /api/v1/products/{id}/items  

Swagger UI:
