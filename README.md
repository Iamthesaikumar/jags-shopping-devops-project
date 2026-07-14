# 🛒 Jags Shopping – End-to-End DevOps Project

## 📌 Project Overview

This project demonstrates an end-to-end deployment of a web application on AWS using Docker and Kubernetes.

The application is containerized using Docker, stored in Amazon Elastic Container Registry (Amazon ECR), deployed to Amazon Elastic Kubernetes Service (Amazon EKS), and exposed to the internet using a Kubernetes Service of type **LoadBalancer**.

The project also demonstrates a **Rolling Update Deployment Strategy** by upgrading the application from **Version 1** to **Version 2** without downtime.

---

## 🎯 Project Objectives

- Containerize a web application using Docker.
- Store Docker images in Amazon ECR.
- Deploy the application to Amazon EKS.
- Expose the application using a Kubernetes Service.
- Perform a Rolling Update from Version 1 to Version 2.
- Understand the complete application deployment lifecycle on AWS.

---
# 🛠️ Technologies Used

| Category | Technology |
|----------|------------|
| Cloud Provider | Amazon Web Services (AWS) |
| Compute | Amazon EC2 |
| Containerization | Docker |
| Container Registry | Amazon Elastic Container Registry (ECR) |
| Container Orchestration | Amazon Elastic Kubernetes Service (EKS) |
| Web Server | NGINX |
| Programming Language | HTML |
| Kubernetes Objects | Deployment, ReplicaSet, Pods, Service |
| Deployment Strategy | Rolling Update |
| CLI Tools | Docker CLI, kubectl, AWS CLI |

---

# 🏗️ Project Architecture

```text
Developer
     │
     ▼
Docker Build
     │
     ▼
Docker Image
     │
     ▼
Amazon ECR
     │
     ▼
Amazon EKS
     │
     ▼
Deployment
     │
     ▼
ReplicaSet
     │
     ▼
Pods
     │
     ▼
Service (LoadBalancer)
     │
     ▼
AWS Elastic Load Balancer
     │
     ▼
Users
```
