# 🚀 Kubernetes CI/CD Project

## 📌 Project Overview
This project demonstrates an end-to-end DevOps pipeline using Docker, Jenkins, and Kubernetes.

## ⚙️ Tech Stack
- Docker
- Jenkins
- Kubernetes
- GitHub
- Flask (Python)

## 🔄 CI/CD Flow
1. Code pushed to GitHub
2. Jenkins triggered via webhook
3. Docker image built
4. Image pushed to Docker Hub
5. Application deployed on Kubernetes

## ☸️ Kubernetes Setup
- Deployment with 3 replicas
- Service (NodePort) for external access
- Load balancing across pods

## 📂 Project Structure
```
Dockerfile
Jenkinsfile
webapp.py
deployment.yaml
service.yaml
README.md
```

## ▶️ How to Run
### Apply Deployment
```
kubectl apply -f deployment.yaml
```

### Apply Service
```
kubectl apply -f service.yaml
```

### Access Application
```
kubectl get svc
```

## 📈 Features
- Automated CI/CD pipeline
- Docker containerization
- Kubernetes deployment and scaling
- Load balancing

## 🏆 Outcome
Successfully built a scalable and automated deployment system using Kubernetes and DevOps tools.
