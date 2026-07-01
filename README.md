# Using Docker Compose to Deploy a Flask Web App with Redis

## 📌 Project Overview

This project demonstrates how to deploy a multi-container application using **Docker Compose**.

The application consists of:

- **Flask** as the web application
- **Redis** as the database/cache
- **Docker Compose** to orchestrate multiple containers

The Flask application connects to Redis to store and retrieve the number of visits to the website.

---

## 🏗 Architecture

```
+-------------+
|   Browser   |
+------+------+
       |
       v
+-------------+
| Flask App   |
+------+------+
       |
       v
+-------------+
| Redis       |
+-------------+
```

---

## 🛠 Technologies Used

- Docker
- Docker Compose
- Python Flask
- Redis
- Git
- GitHub

---

## 📂 Project Structure

```
.
├── app.py
├── requirements.txt
├── Dockerfile
├── compose.yaml
└── README.md
```

---

## 🚀 Build and Run

Build the containers:

```bash
docker compose build
```

Start the application:

```bash
docker compose up
```

Run in detached mode:

```bash
docker compose up -d
```

Stop the application:

```bash
docker compose down
```

---

## 🌐 Access the Application

Open your browser and visit:

```
http://localhost:9000
```

Each page refresh increments the visitor counter stored in Redis.

---

## 📷 Screenshots

### Application Running

<img width="1359" height="767" alt="website-works" src="https://github.com/user-attachments/assets/dc93c0c2-7edd-457a-a3c0-a33b0dc761bf" />



### Running Containers

<img width="1308" height="204" alt="containers-running-successfully" src="https://github.com/user-attachments/assets/fa54d642-3759-4b8f-bb47-592c748f8ec7" />


---

## 📚 What I Learned

- Creating Docker images using Dockerfile
- Running multiple containers using Docker Compose
- Service-to-service communication
- Docker networking
- Volume management
- Container orchestration basics
- Building and deploying multi-container applications

---

## 📖 Useful Docker Compose Commands

```bash
docker compose up -d
docker compose down
docker compose ps
docker compose logs
docker compose restart
docker compose build
docker compose pull
```

---

## 👨‍💻 Author

**Mahmoud Saeed**

GitHub: https://github.com/mahmoudsaeed152687
