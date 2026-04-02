# 🏋️‍♂️ FitTrack Pro API  

## 🚀 Production-Ready Fitness Tracking & Recommendation Backend  

---

## 📌 Overview  

**FitTrack Pro API** is a production-grade backend application built using **Spring Boot** that allows users to track fitness activities and receive personalized recommendations.  

It features **secure JWT authentication**, **role-based authorization**, and **Docker containerization**, making it scalable and ready for real-world deployment.

---

## ✨ Key Features  

### 🔐 Authentication & Security  
- JWT-based authentication  
- Secure login & registration  
- Role-based access (**USER / ADMIN**)  
- Password encryption using BCrypt  

### 🏃 Activity Tracking  
- Log fitness activities (Running, Cycling, etc.)  
- Store dynamic metrics using JSON  
- Fetch user-specific activity history  
- Automatic timestamps  

### 🤖 Recommendation System  
- Generate personalized fitness recommendations  
- Includes:
  - Improvements  
  - Suggestions  
  - Safety tips  
- Fetch by user or activity  

---

## 🧠 Architecture  


Controller → Service → DTO → Entity → Repository → Database


✔ Clean layered architecture  
✔ DTO-based design  
✔ JPA relationships  
✔ JSON column support  
✔ Global exception handling  

---

## 🛠️ Tech Stack  

| Category | Technology |
|----------|-----------|
| Backend  | Java 23, Spring Boot |
| Security | Spring Security + JWT |
| Database | PostgreSQL |
| API Docs | Swagger (OpenAPI 3) |
| Build Tool | Maven |
| Container | Docker |

---

## 📘 API Documentation  

👉 Access Swagger UI:  

http://localhost:8080/swagger-ui.html


---

## ⚙️ Run Locally  

```bash
git clone https://github.com/your-username/fittrack-pro-api.git
cd fittrack-pro-api
mvn clean install
mvn spring-boot:run
🐳 Run with Docker
docker build -t fittrack-api .
docker run -p 8080:8080 fittrack-api
🐘 Database Setup
spring.datasource.url=jdbc:postgresql://localhost:5432/fitness
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
🔌 API Endpoints
🔐 Auth
POST /api/auth/register
POST /api/auth/login
🏃 Activities
POST /api/activities
GET /api/activities
🤖 Recommendations
POST /api/recommendation/generate
GET /api/recommendation/user/{userId}
GET /api/recommendation/activity/{activityId}
🎯 Learning Outcomes
Built secure JWT authentication system
Implemented Spring Security filters
Designed scalable REST APIs
Modeled complex JPA relationships
Used JSON fields in database
Integrated Swagger documentation
Containerized application using Docker
⚠️ Important Note

Ensure sensitive data like passwords are not exposed in API responses.

📈 Future Improvements
Add frontend (React)
Deploy on AWS / Render
Add unit testing
Implement refresh tokens
Convert to microservices
🤝 Contributing

Contributions are welcome! Feel free to fork and improve.

📜 License

Apache 2.0 License
