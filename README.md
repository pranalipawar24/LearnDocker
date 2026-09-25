# 🐳 LearnDocker

A simple **Node.js + MongoDB application** built to understand the fundamentals of Docker and containerization.

> 🚀 From application → Docker image → container → database

---

## 📌 About the Project

This project demonstrates how a Node.js application and MongoDB can be used with Docker.

I created this project to get hands-on experience with:

- 🐳 Docker Images & Containers
- 📦 Dockerfile
- 🔌 Port Mapping
- 🍃 MongoDB Container
- 🖥️ Mongo Express
- ⚙️ Docker Compose
- 🚫 `.dockerignore` & `.gitignore`

---

## 🏗️ How It Works

```text
              Dockerfile
                  │
                  ▼
          ┌───────────────┐
          │  Docker Image │
          └───────┬───────┘
                  │
                  ▼
          ┌───────────────┐
          │ Node.js       │
          │ Container     │
          └───────┬───────┘
                  │
                  ▼
          ┌───────────────┐
          │   MongoDB     │
          │   Container   │
          └───────┬───────┘
                  │
                  ▼
          ┌───────────────┐
          │ Mongo Express │
          └───────────────┘
---

The **Dockerfile** contains the instructions required to package the Node.js application.

Docker uses the Dockerfile to create an **image**, and the image is used to run the application inside a **container**.

MongoDB runs separately, while **Mongo Express** provides a simple web interface to view the database.

---

# 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| 🟢 Node.js | Backend |
| ⚡ Express.js | Web Server |
| 🍃 MongoDB | Database |
| 🖥️ Mongo Express | Database UI |
| 🐳 Docker | Containerization |
| ⚙️ Docker Compose | Manage Containers |
| 🌐 HTML/CSS | Frontend |

---

# 🚀 Docker Workflow

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

▶️ Run the Project

Build the Docker image:

docker build -t docker-testapp .

Run the application:

docker run -d -p 5050:5050 --name docker-testapp docker-testapp

Start MongoDB and Mongo Express:

docker compose -f mongodb.yaml up -d
🌐 Access

Application:
http://localhost:5050

Mongo Express:
http://localhost:8081

📂 Project Structure
LearnDocker/
│
├── public/
├── server.js
├── package.json
├── Dockerfile
├── mongodb.yaml
├── .dockerignore
├── .gitignore
└── README.md
🎯 Learning Goal

The main goal of this project is to understand how Docker can be used to package, run, and manage applications and databases in isolated containers.
