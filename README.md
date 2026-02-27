# 🐳 Docker + NGINX Reverse Proxy Multi-App Architecture

This project demonstrates a **production-style multi-container architecture** using:

- Docker
- Docker Compose
- NGINX Reverse Proxy
- Node.js Applications

---

## 📌 Project Overview

This setup contains:

- 🔹 App1 (Node.js)
- 🔹 App2 (Node.js)
- 🔹 NGINX Reverse Proxy
- 🔹 Docker Compose Orchestration

Traffic routing:

- `/app1` → App1 Container
- `/app2` → App2 Container

---

## 🏗 Architecture

**![](/img/diagram.png)**


---

## 🛠 Technologies Used

- Docker
- Docker Compose
- NGINX
- Node.js
- Linux (EC2)

---

## 📂 Project Structure
```
reverse-proxy-app/
│
├── app1/
│ ├── Dockerfile
│ └── server.js
│
├── app2/
│ ├── Dockerfile
│ └── server.js
│
├── nginx/
│ └── nginx.conf
│
└── docker-compose.yml
```

---

## 🚀 How to Run

### 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/docker-nginx-reverse-proxy-multi-app.git
cd docker-nginx-reverse-proxy-multi-app
```
### 2️⃣ Build and Run Containers
```
docker-compose up -d --build
```

### 3️⃣ Access Applications
```
http://<server-ip>/app1
http://<server-ip>/app2
```

## 🔥 Key Learnings

- ✔ Multi-container communication
- ✔ Reverse Proxy configuration
- ✔ Docker networking
- ✔ Docker Compose orchestration
- ✔ Production-style routing

## 📸 Screenshots

### Docker compose Build
![](/img/Screenshot%20(1201).png)
![](/img/Screenshot%20(1202).png)

### Docker ps output
![](/img/Screenshot%20(1203).png)

### /app1 working
![](/img/Screenshot%20(1206).png)

### /app2 working
![](/img/Screenshot%20(1207).png)

## 👨‍💻 Author

### Vivek Chopade
- DevOps Enthusiast 🚀
- Docker | AWS | Terraform | Ansible | NGINX
