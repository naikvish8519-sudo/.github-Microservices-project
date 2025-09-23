# .github-Microservices-project
🍕 eCommerce Microservices Project  This project is a cloud-native eCommerce platform built using a microservices architecture. It demonstrates full-stack development with .NET 8, React, SQL Server and Azure deployment.
.

📂 Microservices Overview
🛒 Orders Microservice

Manages customer orders and order items.

Uses MongoDB (NoSQL) or SQL Server for persistence.

Provides REST APIs for create, update, delete, and search operations.

Swagger/OpenAPI available for API exploration.

📦 Products Microservice

Handles product catalog, categories, and pricing.

Built with .NET 8, EF Core, and SQL Server.

Supports CRUD operations and integrates with Orders service.

👤 Users Microservice

Manages user registration, authentication, and roles.

Implements JWT-based authentication.

Provides APIs for login, registration, and profile management.

🍕 React Pizza Frontend

React 18 app for frontend ordering experience.

Features:

Browse pizzas & toppings dynamically (via Products API).

Cart management with local + DB persistence (via Orders API).

User login/registration (via Users API).

Deployed to Azure Web App.

🛠️ Tech Stack

Backend:

.NET 8 (ASP.NET Core Web API)

EF Core (SQL Server)

MongoDB Driver

Frontend:

React 18, Hooks, Context API

TailwindCSS / Bootstrap

Database:

SQL Server (Products/Users)

MongoDB (Orders)

DevOps / Cloud:

Docker & Docker Compose

GitHub Actions CI/CD

Azure App Service & AKS

API Gateway: Ocelot

🚀 Getting Started
Prerequisites

.NET 8 SDK

Node.js 18+

SQL Server

MongoDB

Docker
 (for containerized setup)

Clone Repositories


https://github.com/<org-name>/OrdersMicroservice.git

https://github.com/<org-name>/ProductMicroservice.git

https://github.com/<org-name>/UsersMicroservice.git

https://github.com/<org-name>/ReactPizza.git

Running Locally
Backend (example for Orders service)
cd OrdersMicroservice
dotnet restore
dotnet run


API available at:
👉 http://localhost:5043/swagger

Frontend
cd ReactPizza
npm install
npm start


Frontend available at:
👉 http://localhost:3000

📦 Docker Setup

Each microservice has its own Dockerfile.
You can run everything with Docker Compose:

docker-compose up --build

🔄 CI/CD with GitHub Actions

Each repo has a .github/workflows/deploy.yml file.

Workflows:

Build & Test (.NET/React)

Publish artifacts

Deploy to Azure App Service

☁️ Deployment

Backend Microservices: Deployed to Azure App Services.

Frontend (ReactPizza): Deployed to Azure Web App.

Networking: API Gateway (Ocelot) routes requests across services.

Future-ready: Can migrate to Azure Kubernetes Service (AKS) for scaling.

📖 API Endpoints
Orders Microservice

GET /api/Orders

POST /api/Orders

GET /api/Orders/search/orderid/{id}

DELETE /api/Orders/{id}

Pizza Orders (specialized orders)

GET /api/PizzaOrders/search/userid/{userId}

POST /api/PizzaOrders

PUT /api/PizzaOrders/{orderId}

(Swagger docs available at /swagger for each service)

📌 Future Enhancements

Add Payment Microservice (Stripe/Braintree).

Add Inventory & Notifications services.

Deploy on Kubernetes with service mesh (Istio/Linkerd).

Add monitoring with Prometheus + Grafana.
