# 🛒 Ecommerce Backend API (Spring Boot)

This is a backend REST API for an Ecommerce web application built using Spring Boot. It provides a complete system for managing products with clean architecture and MySQL database integration. The backend is designed to work with any frontend like React or Angular and follows MVC architecture for scalability, maintainability, and real-world production structure.

## 🚀 Features
- Full CRUD operations for products (Create, Read, Update, Delete)
- RESTful API built using Spring Boot
- MySQL database integration for persistent storage
- Spring Data JPA for simplified database handling
- Hibernate ORM for object-relational mapping
- MVC layered architecture (Controller → Service → Repository)
- Cross-Origin Resource Sharing (CORS) enabled for frontend communication
- JSON request and response handling
- Scalable and production-ready backend structure
- Easy integration with frontend applications

## 🛠️ Tech Stack
Java, Spring Boot, Spring Data JPA, Hibernate, MySQL, Maven

## 📁 Project Structure
src/
 ├── controller/   → Handles HTTP requests (REST APIs)
 ├── service/      → Business logic layer
 ├── repository/   → Database interaction layer (JPA)
 ├── model/        → Entity classes (Database tables mapping)
 └── resources/
      └── application.properties → Configuration file

## ⚙️ Setup Instructions

1. Clone the repository  
   git clone https://github.com/SyedAbbasMehdi/Ecommerce_Backend.git

2. Import project  
   Open in IntelliJ IDEA or Eclipse as a Maven project

3. Create MySQL database  
   ecommerce_db

4. Configure application.properties
   spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
   spring.datasource.username=root
   spring.datasource.password=your_password
   spring.jpa.hibernate.ddl-auto=update
   spring.jpa.show-sql=true
   spring.jpa.properties.hibernate.format_sql=true

5. Run application  
   mvn spring-boot:run

## 📡 API Endpoints
GET    /api/products        → Get all products
GET    /api/products/{id}   → Get product by ID
POST   /api/products        → Add new product
PUT    /api/products/{id}   → Update product
DELETE /api/products/{id}   → Delete product

## 📦 Sample JSON
{
  "name": "iPhone 15",
  "brand": "Apple",
  "category": "Smartphones",
  "price": 99999,
  "quantity": 10,
  "available": true
}

## 🧠 Key Concepts Used
REST API Development, Spring Boot Dependency Injection, Spring Data JPA, Hibernate ORM, MVC Architecture, MySQL Database Handling, JSON Request/Response, Layered Backend Design

## 🔮 Future Improvements
JWT Authentication, User Login System, Role-based Access (Admin/User), Cart & Order System, Payment Gateway Integration, Product Image Upload, Swagger API Documentation, Cloud Deployment (Render/AWS)

## 👨‍💻 Author
Syed Abbas Mehdi — Full Stack Developer (Learning Phase 🚀)

## ⭐ Note
This is a learning-based full-stack Ecommerce backend project designed to improve backend development skills and build real-world API experience.
