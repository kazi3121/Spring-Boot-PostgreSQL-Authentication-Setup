# Spring Boot with PostgreSQL and Basic Authentication

## Project Description
This is a Spring Boot application that demonstrates basic authentication with PostgreSQL database integration. It includes user management with role-based access control and secure REST endpoints.

## Setup Instructions
- Ensure you have Java 17 and Maven installed
- Install and set up PostgreSQL
- Create a database named `intern_db`
- Update `application.properties` with your PostgreSQL credentials
- Run the application:


## Running the Application
- Use a REST client (e.g., Postman) to test the endpoints
- Public endpoint: `GET http://localhost:8080/public`
- User endpoint: `GET http://localhost:8080/user` (requires authentication)
- Admin endpoint: `GET http://localhost:8080/admin` (requires ADMIN role)
- Create user: `POST http://localhost:8080/users` (requires ADMIN role)

## Credentials
- User: `intern` / Password: `password123` (Role: USER)
- Admin: `admin` / Password: `admin123` (Role: ADMIN)

## Assumptions
- PostgreSQL is running on localhost:6022
- Database credentials are set to default postgres/postgres
- Application runs on port 8080

## Bonus Features Implemented
- Input validation using Jakarta Validation
- Global exception handling for validation errors and duplicate usernames
- Basic unit test setup
