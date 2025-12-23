# Fitness App Microservices

A modern **full-stack fitness application** built using **microservices architecture**.  
This project demonstrates how to structure and deploy scalable fitness services using Spring Boot, Eureka, API Gateway, Config Server, and React. Services are independently deployable and communicate via REST APIs.
---
## 🚀 About the Project

Fitness App Microservices is a production-oriented project that enables users to:

- Register & authenticate securely  
- Log fitness activities  
- Retrieve personalized fitness data  
- Explore services via API Gateway  
- Scale microservices independently  

Architecture highlights:
✔ Spring Boot based microservices  
✔ API Gateway for routing  
✔ Eureka for service discovery  
✔ Central Config Server  
✔ Frontend app for user interaction  
✔ Docker friendly setup

---

## 🧱 Project Structure

| Module | Description |
|--------|-------------|
| **configserver** | Centralized configuration management |
| **eureka** | Service registry for discovery |
| **gateway** | API Gateway to expose all services |
| **userservice** | User registration & authentication |
| **activityservice** | Fitness activity tracking |
| **aiservice** | AI recommendation / analytics (if applicable) |
| **fitness-app-frontend** | React frontend UI |
| **README.md** | This documentation |

---

## 📦 Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | Spring Boot, Spring Cloud |
| Discovery | Eureka Server |
| Routing | Spring Cloud Gateway |
| Config | Spring Cloud Config Server |
| UI | React.js |
| Build Tools | Maven / Gradle |
| Deployment | Docker (optional) |

---

## ⚙️ Getting Started

### 1️⃣ Clone Repo
```bash
git clone https://github.com/saksham869/fitness-app-microservices.git
cd fitness-app-microservices
2️⃣ Run Services
With IntelliJ / IDE
Open the project

Run each module:
configserver, eureka, gateway, userservice, activityservice, aiservice

Or using Maven
bash
Copy code
cd configserver && mvn spring-boot:run
cd eureka && mvn spring-boot:run
cd gateway && mvn spring-boot:run
cd userservice && mvn spring-boot:run
cd activityservice && mvn spring-boot:run
cd aiservice && mvn spring-boot:run
3️⃣ Frontend (React)
bash
Copy code
cd fitness-app-frontend
npm install
npm start
🛠 Features
✔ Centralized configuration
✔ Client-side routing with API Gateway
✔ Service discovery with Eureka
✔ REST API endpoints per service
✔ Scalable microservices design
✔ Separate frontend UI

🗂 API Endpoints
Example endpoints (adjust based on your code)

Authentication

bash
Copy code
POST /userservice/api/v1/auth/register
POST /userservice/api/v1/auth/login
Activities

bash
GET /activityservice/api/v1/activities
POST /activityservice/api/v1/activities
Gateway Proxy

bash
http://localhost:8080/userservice/**
http://localhost:8080/activityservice/**
📌 Environment Variables
Make sure to configure:
📁 .gitignore
gitignore
Copy code
*.iml
.idea/
target/
node_modules/
.env
logs/
✨ Contributing
Want to improve this project?

Fork the repository

Create your feature branch

Commit & push

Open a pull request 🚀

👤 Contact
Created by Saksham — feel free to reach out if you’d like help scaling this further 🚀
