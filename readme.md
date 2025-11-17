
## 📘 README.md for `assignment11`

# 🧮 Assignment11: FastAPI Calculator App

This project is a FastAPI-based calculator API developed for NJIT's CS601 Assignment 11. It supports basic arithmetic operations and is fully containerized with Docker, integrated with PostgreSQL, and deployed via GitHub Actions to Docker Hub.

---

## 🚀 Features

- FastAPI backend with RESTful endpoints
- PostgreSQL database integration
- pgAdmin for DB visualization
- Dockerized with `docker-compose`
- CI/CD pipeline using GitHub Actions
- Trivy vulnerability scanning
- Automatic image push to Docker Hub

---

## 🛠️ Local Development Setup

### Prerequisites

- Docker & Docker Compose installed
- Python 3.10+ (for local testing)

### Run Locally

```bash
git clone https://github.com/DanaTryon/assignment11.git
cd assignment11
docker-compose up --build
```

Access the app at: [http://localhost:8000](http://localhost:8000)  
Swagger docs: [http://localhost:8000/docs](http://localhost:8000/docs)  
pgAdmin: [http://localhost:5050](http://localhost:5050)

---

## ✅ API Endpoints

| Method | Endpoint         | Description              |
|--------|------------------|--------------------------|
| GET    | `/`              | Serve the index.html template     |
| POST   | `/calculate`     | Perform arithmetic       |

---

## 🧪 Running Tests Locally
Activate your virtual environment and run:

```bash
# From the root directory
pytest
```
This will discover and run all tests in the tests/ directory.

---

## 🐳 Docker Hub

This project is automatically deployed to Docker Hub:

**Image:** [`danatryon/assignment11`](https://hub.docker.com/r/danatryon/assignment11)  
To pull the image manually:

```bash
docker pull danatryon/assignment11:latest
```

---

## 🔄 CI/CD Pipeline

GitHub Actions workflow includes:

- ✅ Unit, integration, and e2e tests
- 🔐 Trivy security scan
- 📦 Docker image build and push
- 🚀 Deployment on push to `main`



