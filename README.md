# 🚀 Node Express Dockerized Application

This project demonstrates how to **build, containerize, and run a Node.js Express application using Docker**, making it portable, lightweight, and easy to deploy across environments.

---

## ✅ Features

* Simple **Express.js REST API**
* Multiple routes for testing and monitoring
* Fully **Dockerized** application
* Support for **environment variables**
* Lightweight **Alpine-based Node image**
* Clean and beginner-friendly project structure

### Available API Endpoints

* `/` – Home route
* `/about` – About information
* `/status` – Application status
* `/health` – Health check endpoint

---

## 📂 Project Structure

```text
node-app/
│
├── app.js              # Main application file
├── package.json        # Node.js dependencies & scripts
├── Dockerfile          # Docker build instructions
├── .dockerignore       # Files ignored by Docker
└── public/             # Static assets (if any)
```

---

## 🔧 Prerequisites

Make sure the following are installed on your system:

1. **Node.js** (for running locally)
2. **Docker** (for containerization)
3. **Git** (to clone the repository)

---

## 📥 Clone This Repository

To clone this repository to your local system:

```bash
git clone https://github.com/aakansha113/Node-Express-Dockerized-Application.git
cd Node-Express-Dockerized-Application
```

---

## 🛠 Step 1: Install Dependencies (Local)

```bash
npm install
```

---

## ▶️ Step 2: Run the Application Locally

```bash
npm start
```

Access the application in your browser:

```text
http://localhost:5000
```

---

## 🐳 Step 3: Dockerize the Application

### ✅ Build Docker Image

```bash
docker build -t node-app:v1 .
```

---

### ▶️ Run Docker Container

```bash
docker run -dit --name node-container -p 5000:5000 node-app:v1
```

Verify running containers:

```bash
docker ps
```

---

## 🌐 Access the Application

You can access the application using a browser or `curl`:

```bash
curl http://localhost:5000/
curl http://localhost:5000/about
curl http://localhost:5000/health
curl http://localhost:5000/status
```

Or open directly in browser:

```text
http://localhost:5000/
http://localhost:5000/about
http://localhost:5000/health
http://localhost:5000/status
```

---

## 🧹 Cleanup (Optional)

Stop and remove the container:

```bash
docker stop node-container
docker rm node-container
```

Remove the image:

```bash
docker rmi node-app:v1
```

---

## 🎯 Key Learnings

* Building REST APIs using Express.js
* Dockerizing Node.js applications
* Using Alpine-based images for smaller size
* Running and managing containers

---

## 👩‍💻 Author

**Akshu Hujare**
Aspiring DevOps Engineer 🚀

---

## ⭐ Show Your Support

If you like this project, feel free to **⭐ star the repository** and share it!
