# AWS EC2 Docker Deployment with Public URL
This project demonstrates a production-ready Docker deployment on AWS EC2 using Docker Compose and Nginx.

## Architecture
Internet → EC2 → Nginx → Docker App

## Prerequisites
- AWS EC2 instance (Ubuntu 20.04+)
- Docker & Docker Compose installed
- Ports 80 and 22 open

## Setup Instructions

### 1. Clone Repository
```bash
git clone https://github.com/<your-username>/aws-ec2-docker-public-url.git
cd aws-ec2-docker-public-url
```

### 2. Start Containers
```bash
docker compose up -d --build
docker ps
```

### 3. Access Application
```cpp
In browser:
http://<EC2-PUBLIC-IP>
```

### 4. Restart/Stop
```bash
docker compose restart
docker compose down
```
