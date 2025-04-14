# 🐳 Kubernetes NGINX Deployment with Minikube

This project demonstrates deploying an NGINX application to a local Kubernetes cluster using Minikube and Docker. It covers fundamental Kubernetes concepts such as deployments, services, scaling, and cluster introspection.

---

## 🚀 Project Objective

To provision, deploy, and manage containerized applications on Kubernetes using Minikube — all through declarative `.yaml` manifests.

---

## 🛠️ Tools Used

- **Kubernetes** (v1.32.0)
- **Minikube** (v1.35.0)
- **Docker** (v27.4.1)
- **kubectl**

---

## 📁 Folder Structure

. ├── deployment.yaml # Kubernetes Deployment definition for NGINX 
. ├── service.yaml # NodePort Service to expose the NGINX app 
. ├── commands.md # CLI commands used for management and testing 
. ├── .gitignore # Basic ignore rules for logs/temp files 
. └── README.md

---

## 🔧 Setup & Usage

1. **Start Minikube**
   ```
   minikube start
   ```

## Deploy the Application
```
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```
## Check Deployments & Pods

```
kubectl get deployments
kubectl get pods
```
Access the App in Browser

```
minikube service nginx-service
Scale the Application

```
kubectl scale deployment nginx-deployment --replicas=3
Clean Up

```
kubectl delete -f deployment.yaml
kubectl delete -f service.yaml
```
## 📌 Key Concepts Learned
- Setting up local Kubernetes using Minikube
- Creating and managing Deployments
- Exposing services using NodePort
- Scaling applications using kubectl

