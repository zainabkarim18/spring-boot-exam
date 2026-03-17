# Product Inventory API

A Spring Boot REST API that manages products in an in‑memory store. Supports full CRUD operations (create, read, update, delete).

## How to Run
./mvnw spring-boot:run

## API Endpoints

| Method | URL                  | Description                          |
|--------|----------------------|--------------------------------------|
| GET    | `/api/products`      | Get all products                     |
| GET    | `/api/products/{id}` | Get a product by ID                  |
| POST   | `/api/products`      | Create a new product                 |
| PUT    | `/api/products/{id}` | Update an existing product by ID     |
| DELETE | `/api/products/{id}` | Delete a product by ID               |


# Product Management API – curl Examples

## Create a product
curl -X POST http://localhost:8080/api/products -H "Content-Type: application/json" -d "{\"name\":\"Laptop\",\"category\":\"Electronics\",\"price\":999.99,\"quantity\":10}" -v

## Get all products
curl http://localhost:8080/api/products

## Get product by ID
curl http://localhost:8080/api/products/1

## Update a product
curl -X PUT http://localhost:8080/api/products/1 -H "Content-Type: application/json" -d "{\"name\":\"Laptop Pro\",\"category\":\"Electronics\",\"price\":1299.99,\"quantity\":5}" -v



## Delete a product
curl -X DELETE http://localhost:8080/api/products/1

