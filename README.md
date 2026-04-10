# Product Service

Product catalog management service for the ecommerce platform.

## Port
- **8082**

## Description
Handles product CRUD operations, inventory management, and product search with Redis caching.

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/products | Create product |
| GET | /api/products | Get all products |
| GET | /api/products/available | Get available products |
| GET | /api/products/category/{category} | Get products by category |
| GET | /api/products/search?name= | Search products |
| GET | /api/products/{id} | Get product by ID |
| PUT | /api/products/{id} | Update product |
| PUT | /api/products/{id}/stock | Update stock |
| DELETE | /api/products/{id} | Delete product |

## Running the Service

```bash
mvn spring-boot:run
```

## Dependencies
- MySQL Database: `ecommerce_product`
- Redis: localhost:6379
- Eureka Server: http://localhost:8761
