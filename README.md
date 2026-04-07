# 🚀 Self-Healing Infrastructure with Chaos Engineering & Monitoring

## 📌 Project Overview

This project demonstrates a **self-healing infrastructure system** using Kubernetes.
It showcases how modern DevOps systems automatically recover from failures, monitor health, and trigger alerts.

---

## 🧠 Key Features

* 🔹 Containerized application using Docker
* 🔹 Kubernetes Deployment with self-healing capability
* 🔹 Monitoring using Prometheus
* 🔹 Alerting based on pod failures
* 🔹 Chaos Engineering using Chaos Mesh
* 🔹 Automatic recovery from failures

---

## 🏗️ Architecture

```
User Request
     ↓
Kubernetes Cluster (Minikube)
     ↓
Pods (Application)
     ↓
Prometheus (Monitoring)
     ↓
Alert Manager (Alerts)
     ↓
Chaos Mesh (Failure Injection)
```

---

## ⚙️ Tech Stack

* Docker
* Kubernetes (Minikube)
* Prometheus
* Chaos Mesh
* Node.js (Express)

---

## 🚀 Setup Instructions

### 1️⃣ Start Minikube

```
minikube start --driver=docker
```

### 2️⃣ Build Docker Image

```
docker build -t self-healing-app .
```

### 3️⃣ Deploy to Kubernetes

```
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

### 4️⃣ Check Pods

```
kubectl get pods
```

---

## 📊 Monitoring (Prometheus)

```
kubectl port-forward svc/prometheus-server 9090:80
```

Open: http://localhost:9090

---

## 🚨 Alerting

* Detects high pod restart count
* Triggers alert when failures occur

---

## 💥 Chaos Engineering

* Simulates pod failures
* Automatically kills pods
* Tests system resilience

---

## 🔄 Self-Healing Flow

1. Chaos Mesh kills a pod
2. Kubernetes recreates it
3. Prometheus detects restart
4. Alert is triggered

---

## 📈 Outcome

* Built a resilient system
* Demonstrated automatic recovery
* Applied real-world DevOps practices

---

## 🔮 Future Enhancements

* Cloud deployment (Azure / AWS)
* CI/CD pipeline
* Grafana dashboards

---

## 👩‍💻 Author

Mokshitha K
B.Tech Student | DevOps Enthusiast

---

## ⭐ Key Learning

Designed a complete self-healing system with monitoring, alerting, and chaos testing.
