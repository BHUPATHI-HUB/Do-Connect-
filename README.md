
# DoConnect_Manideep - API Backend Service

This is the backend API module for **DoConnect**, a Question & Answer platform similar to Stack Overflow. This Spring Boot-based microservice handles core backend functionalities such as user authentication, posting questions and answers, and moderation support.

---

## 🛠️ Tech Stack

- Java 17
- Spring Boot
- Spring MVC
- Spring Security (JWT-based)
- Hibernate & JPA
- MySQL / H2
- Maven

---

## 📁 Project Structure

Doconnect_Manideep/
├── Api/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   └── resources/
│   ├── pom.xml
│   └── mvnw, .gitignore, etc.

---

## 🚀 Features

- ✅ User Registration & Login
- ✅ JWT Token Authentication
- ✅ Ask / Answer / Comment on Questions
- ✅ Admin Moderation Panel (for question/answer/comment approval)
- ✅ Role-based access control
- ✅ Swagger API Documentation (if enabled)

---

## 🧪 API Endpoints (Example)

| HTTP Method | Endpoint                    | Description                  |
|-------------|-----------------------------|------------------------------|
| POST        | /portal/auth/login          | Authenticate user            |
| POST        | /portal/register            | Register a new user          |
| GET         | /portal/questions           | Get all approved questions   |
| POST        | /portal/questions/ask       | Ask a new question           |
| POST        | /portal/answers/post        | Post an answer               |
| GET         | /adminsonly/users           | Admin: View all users        |
| GET         | /adminsonly/questions       | Admin: Review questions      |

---

## 🧾 How to Run the Project

Step 1: Navigate to the project directory
```bash
cd Doconnect_Manideep/Api
```

Step 2: Build the project
```bash
./mvnw clean install
```

Step 3: Run the Spring Boot application
```bash
./mvnw spring-boot:run
```

> By default, the app will run on http://localhost:8080.

---

## 🔐 Security

- JWT-based Authentication for secured endpoints
- Role-based access (`USER`, `ADMIN`)
- Session handling with token expiry

---

## 📦 Database Setup

- Use H2 (in-memory) for dev/testing.
- Use MySQL for production (update in `application.properties`).

---

## 🧰 Dependencies

<dependencies>
  Spring Boot Starter Web
  Spring Boot Starter Security
  Spring Boot Starter Data JPA
  MySQL Driver / H2
  JWT (jjwt)
</dependencies>

---

## 📄 License

This project is developed as part of internal learning and submission. All rights reserved by **Bhupathi Manideep**.

---

## 🙋‍♂️ Author

**Bhupathi Manideep**  
Software Developer | Java | Spring Boot | Microservices  
Final Project – DoConnect
