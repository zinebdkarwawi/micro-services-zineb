# Microservices Project (Zineb Edition)

This project consists of 5 microservices:
1.  **Discovery Service** (Eureka)
2.  **Config Service**
3.  **Customer Service**
4.  **Inventory Service**
5.  **Billing Service**
6.  **Gateway Service**

## 🚀 How to Run

### 1. Prerequisites
*   Java 17 or 21
*   Maven

### 2. Startup Order
1.  **Discovery Service** (Port 8761)
2.  **Config Service** (Port 8888)
3.  **Customer Service** (Port 8080)
4.  **Inventory Service** (Port 8081)
5.  **Billing Service** (Port 8082)
6.  **Gateway Service** (Port 8887)

## ⚠️ Important Configuration Setup (After Cloning)

The `config-repo` folder serves as the source for the Config Service. Because this project is stored in a single repository, the inner Git configuration of `config-repo` might not be preserved when you clone it.

**If you clone this project on a new machine, you MUST run these commands to fix the Config Server:**

```bash
cd config-repo
git init
git add .
git commit -m "Initialize config"
cd ..
```

Then you can start `Config-Service`.
