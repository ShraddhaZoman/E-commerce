# E-Commerce Website

This is a **full-stack e-commerce application** built using **Angular** for the frontend and **Spring Boot** for the backend. The application allows users to browse products, add them to a cart, and proceed with checkout.

## Features
- Product listing and filtering
- User authentication (Register/Login)
- Shopping cart management
- Order placement and checkout
- Secure API endpoints with Spring Security
- Uses **MySQL** as the database
- Backend built with **Spring Boot and REST API**
- Frontend built with **Angular**

## Tech Stack
- **Frontend**: Angular
- **Backend**: Spring Boot, Spring Data REST
- **Database**: MySQL
- **Security**: JWT authentication
- **ORM**: Hibernate/JPA

---

## Getting Started
### 1. Clone the Repository
```sh
git clone https://github.com/yourusername/ecommerce-app.git
cd ecommerce-app
```

### 2. Backend Setup (Spring Boot)
#### Install Dependencies
```sh
cd backend
mvn clean install
```
#### Configure MySQL Database
Update `application.properties` in the `src/main/resources` folder:
```
spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
```
#### Run the Backend Server
```sh
mvn spring-boot:run
```

### 3. Frontend Setup (Angular)
#### Install Dependencies
```sh
cd frontend
npm install
```
#### Run the Frontend Server
```sh
ng serve
```

### 4. API Endpoints
- **Products**
  - `GET /api/products` - Get all products
  - `GET /api/products/{id}` - Get product by ID
- **Categories**
  - `GET /api/categories` - Get all categories
- **User Authentication**
  - `POST /api/auth/register` - Register a new user
  - `POST /api/auth/login` - Login user
- **Shopping Cart & Orders**
  - `POST /api/cart/add` - Add item to cart
  - `POST /api/orders` - Place an order

---

## Project Structure
```
ecommerce-app/
├── backend/
│   ├── src/main/java/com/code/spring_pro/
│   │   ├── config/
│   │   │   ├── MyDataRestConfig.java
│   │   ├── entity/
│   │   │   ├── Product.java
│   │   │   ├── ProductCategory.java
│   │   ├── repository/
│   │   │   ├── ProductRepository.java
│   │   │   ├── ProductCategoryRepository.java
│   │   ├── service/
│   │   ├── controller/
│   ├── pom.xml
│
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   │   ├── components/
│   │   │   ├── services/
│   │   │   ├── models/
│   │   ├── assets/
│   ├── angular.json
│   ├── package.json
│
└── README.md
```

## License
This project is open-source and available under the MIT License.

---

## Contributing
Feel free to fork this repository and make improvements. Pull requests are welcome!

---

### Contact
If you have any issues or questions, feel free to reach out!

