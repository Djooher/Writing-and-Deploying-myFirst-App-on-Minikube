# Writing-and-Deploying-myFirst-App-on-Minikube
# 🚀 Flask Kubernetes Minikube Project

## 📌 Description
This project demonstrates a complete DevOps workflow using Docker and Kubernetes (Minikube) to deploy a simple Flask application locally.

## 🧰 Tools Used
- WSL (Ubuntu)
- Docker
- Kubernetes (Minikube)
- kubectl
- Flask (simple web app)

## ⚙️ Architecture
Code → Docker Image → Kubernetes Deployment → Service → Browser

## 🚀 How to Run

```bash
docker build -t flask-k8s-app .
minikube image load flask-k8s-app
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
minikube service flask-service --url
