# 🏋️ FitTrack Pro API  
🚀 Production-Ready Fitness Tracking Backend (Spring Boot)

---

## 📌 Overview
FitTrack Pro API is a scalable backend application built using Spring Boot that enables users to track fitness activities and receive personalized recommendations.

It simulates a real-world production backend with secure authentication, modular architecture, and containerized deployment.

---

## ✨ Key Features

### 🔐 Authentication & Security
- JWT-based authentication
- Secure login & registration
- Role-based access control (USER / ADMIN)
- Password encryption using BCrypt

### 🏃 Activity Tracking
- Log fitness activities (Running, Cycling, etc.)
- Store flexible activity data using JSON fields
- Fetch user-specific activity history
- Automatic timestamp management

### 🤖 Recommendation System
- Generate personalized fitness recommendations
- Includes:
  - Improvements
  - Suggestions
  - Safety tips
- Fetch recommendations by user or activity

---

## 🧠 Architecture
Controller → Service → DTO → Entity → Repository → Database  

✔ Clean layered architecture  
✔ DTO-based request/response handling  
✔ JPA relationships  
✔ JSON column support  
✔ Global exception handling  

---

## 🛠️ Tech Stack

| Category     | Technology |
|--------------|-----------|
| Backend      | Java 23, Spring Boot |
| Security     | Spring Security, JWT |
| Database     | PostgreSQL |
| API Docs     | Swagger (OpenAPI 3) |
| Build Tool   | Maven |
| Container    | Docker |

---

## 📘 API Documentation
👉 Swagger UI:  
http://localhost:8080/swagger-ui.html  

---

## ⚙️ Run Locally
```bash
git clone https://github.com/Aman-Niyazi/fittrack-pro-api.git
cd fittrack-pro-api
mvn clean install
mvn spring-boot:run
🐳 Run with Docker
docker build -t fittrack-api .
docker run -p 8080:8080 fittrack-api
🐘 Database Configuration
spring.datasource.url=jdbc:postgresql://localhost:5432/fitness
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
🔌 API Endpoints
🔐 Authentication
POST /api/auth/register
POST /api/auth/login
🏃 Activities
POST /api/activities
GET /api/activities
🤖 Recommendations
POST /api/recommendation/generate
GET /api/recommendation/user/{userId}
GET /api/recommendation/activity/{activityId}
📸 API Preview (Add Screenshots Here 🚨)

👉 Add:

Swagger UI screenshot
Postman response JSON
DB schema (optional)
🎯 Learning Outcomes
Implemented secure JWT authentication system
Designed scalable REST APIs using Spring Boot
Applied layered architecture for clean code structure
Modeled complex JPA relationships
Integrated Swagger for API documentation
Containerized application using Docker
📈 Future Improvements
Add frontend (React)
Deploy on AWS / Render
Add unit & integration testing
Implement refresh tokens
Convert to microservices architecture
🤝 Contributing

Contributions are welcome! Feel free to fork and improve.

📜 License

Apache 2.0 License
