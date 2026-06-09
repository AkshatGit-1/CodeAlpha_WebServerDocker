# 🐳 Web Server using Docker
## CodeAlpha DevOps Internship - Task 4

## 📋 Project Overview
A web server that is running inside a Docker 
container using NGINX.

## 🛠️ Technologies Used
- Docker
- NGINX
- HTML/CSS

## 🚀 How to Run

### Step 1: Build Docker Image
```bash
docker build -t my-web-server .

### Step 2: Run the Container
docker run -d -p 8080:80 --name my-web-container my-web-server

### Step 3: Check the Browser
http://localhost:8080

### Step 4: How to delete and rebuild Docker Image
docker stop my-web-container && docker rm my-web-container && docker rmi my-web-server && docker build -t my-web-server . && docker run -d -p 8080:80 --name my-web-container my-web-server

## Commands for Monitoring

### See the Activity
docker logs my-web-container

### Check the status
docker stats my-web-container
#To Exit
Ctrl+C

###Check Full Details
docker inspect my-web-container
