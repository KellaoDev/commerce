# Commerce

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/KellaoDev)
# About project 

This is a RESTful API developed using Java with the Spring Boot framework. The API allows management of users, products, orders, and categories, providing full CRUD operations for each resource.

## API documentation

### Users

#### Create user

```http
POST {LOCALHOST}/users
```

```json
{
  "name": "string",
  "email": "string",
  "phone": "string",
  "password": "string"
}
```

#### Get all users

```http
GET {LOCALHOST}/users
```

#### Get user by ID

```http
GET {LOCALHOST}/users/{id}
```

#### Update user 

```http
PUT {LOCALHOST}/users/{id}
```

#### Delete user 

```http
DELETE {LOCALHOST}/users/{id}
```

### Products

#### Get all products

```http
GET {LOCALHOST}/products
```

#### Get product by ID

```http
GET {LOCALHOST}/products/{id}
```

### Orders

#### Get all orders

```http
GET {LOCALHOST}/orders
```

#### Get order by ID

```http
GET {LOCALHOST}/orders/{id}
```

### Categories

#### Get all categories

```http
GET {LOCALHOST}/categories
```

#### Get categories by ID

```http
GET {LOCALHOST}/categories/{id}
```

## Technologies used

#### • Java
#### • Spring Framework
#### • H2 / PostgreSQL / Hibernate

## How to execute the project

### Prerequisites:

#### Make sure you have installed:

JDK 17 → java -version

Maven → mvn -version

Database (PostgreSQL)

```bash
# Clone repository
https://github.com/KellaoDev/commerce.git

# Configure database test
In the archive application.properties:
Example(H2)

spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.username=sa
spring.datasource.password=
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.jpa.defer-datasource-initialization=true
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true

# Configure database production
In the archive application.properties:
Example(PostgreSQL)

# Run the project with Maven
mvn spring-boot:run

# Access the API
http://localhost:8080 (or another configured port)
```
## Author

### Kélio Cirilo da Silva Filho
https://www.linkedin.com/in/keliocirilo/







