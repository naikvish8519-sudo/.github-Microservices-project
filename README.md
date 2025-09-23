🍕 Pizza Ordering App

Description:
A full-stack pizza ordering application built with React (frontend) and .NET microservices (backend). Users can browse available pizza sizes, customize their order with veg and non-veg toppings, adjust quantities, and add items to a global shopping cart. The app features a responsive UI, real-time cart updates using React Context, and dynamic price calculations per pizza and for the grand total. It also includes loading states with spinners for better UX. The backend microservices (Products, Users, Orders) are deployed to Azure App Services, and the frontend React app is hosted with integration to these APIs.
🍕 React Pizza Frontend

Purpose: Frontend React app with Pizza Builder, Cart, and Checkout

Live App:
https://react-pizza-gsdtecavejezewfr.canadacentral-01.azurewebsites.net

GitHub Repo:
https://github.com/naikvish8519-sudo/ReactPizza

<img width="1399" height="945" alt="image" src="https://github.com/user-attachments/assets/8c05344d-8ab4-4561-bbdc-54792953328a" />

Pizza Menu & Cart

📂 Microservices Overview
👤 Users Microservice

Purpose: Authentication & User Management

Live Swagger:
https://micro-userservice-h2gtehf8eddpbscd.canadacentral-01.azurewebsites.net

GitHub Repo:
https://github.com/naikvish8519-sudo/UsersMicroservice
<img width="645" height="553" alt="image" src="https://github.com/user-attachments/assets/960938cc-718a-4989-bb4b-3fc21394bc8a" />


📦 Products Microservice

Purpose: Manage Pizza Sizes, Toppings, and Pricing

Live Swagger:
https://micro-productservice-b2g0g5gafpawcsdf.japanwest-01.azurewebsites.net/index.html

GitHub Repo:
https://github.com/naikvish8519-sudo/ProductMicroservice
<img width="1399" height="945" alt="image" src="https://github.com/user-attachments/assets/8c05344d-8ab4-4561-bbdc-54792953328a" />

🛒 Orders Microservice

Purpose: Cart Persistence & Order Checkout

Live Swagger:
micro-orderservice-bnc2gjg2h5emhqby.canadacentral-01.azurewebsites.net

GitHub Repo:
https://github.com/naikvish8519-sudo/OrdersMicroservice

<img width="1042" height="871" alt="image" src="https://github.com/user-attachments/assets/a732175c-87d5-42b1-af19-ed7d40e869e4" />

🛠️ Tech Stack

Frontend: React 18, Context API, Bootstrap/TailwindCSS

Backend: .NET 8 (ASP.NET Core Web API), EF Core, REST APIs

Database: SQL Server (Users/Products), MongoDB (Orders)

Cloud & DevOps: Docker, GitHub Actions CI/CD, Azure App Services

🚀 Features

🔐 Secure login/registration (Users Service)

🍕 Dynamic pizza menu & toppings (Products Service)

🛒 Cart persistence & order history (Orders Service)

☁️ End-to-end deployment on Azure App Services with CI/CD

📦 Deployment

Each microservice deployed independently to Azure App Service

CI/CD pipelines managed with GitHub Actions

React frontend deployed separately to Azure Web App

Configurable via .env (local) and App Settings (Azure)

📌 Future Enhancements

💳 Payment integration (Stripe or Braintree)

☸️ Deployment to Azure Kubernetes Service (AKS) for scalability

📢 Notifications/Email microservice

📊 Monitoring with Application Insights + Grafana



