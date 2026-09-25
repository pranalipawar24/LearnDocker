# 🐳 LearnDocker

A simple **Node.js + MongoDB application** built to understand the fundamentals of **Docker and containerization**.

> 🚀 Application → Docker Image → Container → Database

---

## 📌 About the Project

This project demonstrates how a **Node.js application** and **MongoDB** can be used with Docker.

I created this project to get hands-on experience with:

- 🐳 Docker Images & Containers
- 📦 Dockerfile
- 🔌 Port Mapping
- 🍃 MongoDB with Docker
- 🖥️ Mongo Express
- ⚙️ Docker Compose
- 🚫 `.dockerignore` & `.gitignore`

---

## 🏗️ How It Works

```text
                 Dockerfile
                     │
                     ▼
              ┌─────────────┐
              │ Docker Image│
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │   Node.js   │
              │  Container  │
              └──────┬──────┘
                     │
               Docker Network
                     │
                     ▼
              ┌─────────────┐
              │   MongoDB   │
              │  Container  │
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │Mongo Express│
              └─────────────┘
```

The **Dockerfile** contains the instructions required to package the Node.js application.

Docker uses the Dockerfile to create an **image**, and the image is used to run the application inside a **container**.

MongoDB runs in a separate container, while **Mongo Express** provides a simple web interface to view the database.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| 🟢 Node.js | Backend |
| ⚡ Express.js | Web Server |
| 🍃 MongoDB | Database |
| 🖥️ Mongo Express | Database UI |
| 🐳 Docker | Containerization |
| ⚙️ Docker Compose | Manage Containers |
| 🌐 HTML/CSS | Frontend |

---

## 🚀 Docker Workflow

```text
Code
  ↓
Dockerfile
  ↓
Docker Image
  ↓
Docker Container
  ↓
Running Application
```
---

## 🐳 Docker Hub

The Docker image for this project has been successfully built and pushed to Docker Hub.

**Docker Image:**

```text
You can pull the image directly using:
docker pull pranalipawar/testapp
```
---

## ▶️ Run the Project

### 1️⃣ Build the Docker Image

```bash
docker build -t docker-testapp .
```

### 2️⃣ Run the Application

```bash
docker run -d -p 5050:5050 --name docker-testapp docker-testapp
```

### 3️⃣ Start MongoDB and Mongo Express

```bash
docker compose -f mongodb.yaml up -d
```

---

## 🌐 Access

| Service | URL |
|---------|-----|
| 🌐 Application | http://localhost:5050 |
| 🖥️ Mongo Express | http://localhost:8081 |

---

## 📂 Project Structure

```text
LearnDocker/
│
├── public/
│   ├── index.html
│   └── style.css
│
├── server.js
├── package.json
├── package-lock.json
├── Dockerfile
├── mongodb.yaml
├── .dockerignore
├── .gitignore
└── README.md
```

---

## 🎯 Learning Goal

The main goal of this project is to understand how Docker can be used to **package, run, and manage applications and databases in isolated containers**.

This project provides hands-on experience with:

- Docker Images
- Docker Containers
- Dockerfiles
- Port Mapping
- Docker Compose
- MongoDB
- Mongo Express

---


