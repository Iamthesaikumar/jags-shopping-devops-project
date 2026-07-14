# 🛒 static web application – End-to-End DevOps Deployment on AWS

<p align="center">

![AWS](https://img.shields.io/badge/AWS-EKS-orange?style=for-the-badge&logo=amazonaws)
![Docker](https://img.shields.io/badge/Docker-Container-blue?style=for-the-badge&logo=docker)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-blue?style=for-the-badge&logo=kubernetes)
![Amazon ECR](https://img.shields.io/badge/Amazon-ECR-yellow?style=for-the-badge&logo=amazonaws)
![NGINX](https://img.shields.io/badge/WebServer-NGINX-green?style=for-the-badge&logo=nginx)

</p>

---

# 📖 Project Overview

This project demonstrates an **end-to-end DevOps deployment** of a static web application on **Amazon Web Services (AWS)**.

The application is:

- Containerized using Docker
- Stored in Amazon Elastic Container Registry (ECR)
- Deployed to Amazon Elastic Kubernetes Service (EKS)
- Exposed using Kubernetes Service (LoadBalancer)
- Upgraded using the Rolling Update deployment strategy

This project simulates a real-world DevOps deployment workflow from application development to production deployment.

---

# 🎯 Project Objectives

- Build a Docker image for a web application.
- Push the Docker image to Amazon ECR.
- Deploy the application to Amazon EKS.
- Expose the application using Kubernetes Service.
- Perform Rolling Updates with zero downtime.
- Understand Kubernetes Deployments, ReplicaSets, Pods, Services, and Load Balancers.

---

# 🛠️ Technologies Used

| Category | Technology |
|-----------|------------|
| Cloud | Amazon Web Services (AWS) |
| Compute | Amazon EC2 |
| Containerization | Docker |
| Container Registry | Amazon Elastic Container Registry (ECR) |
| Container Orchestration | Amazon Elastic Kubernetes Service (EKS) |
| Web Server | NGINX |
| Programming | HTML |
| Kubernetes Objects | Deployment, ReplicaSet, Pods, Service |
| Deployment Strategy | Rolling Update |
| CLI Tools | Docker CLI, kubectl, AWS CLI |

---

# 🏗️ Solution Architecture

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
        Amazon Elastic Container Registry
                        │
                        ▼
        Amazon Elastic Kubernetes Service
                        │
                        ▼
                 Kubernetes Deployment
                        │
                        ▼
                   ReplicaSet
                        │
                        ▼
                     Pods (2)
                        │
                        ▼
          Kubernetes Service (LoadBalancer)
                        │
                        ▼
           AWS Elastic Load Balancer (ELB)
                        │
                        ▼
                     End Users
```

---

# 🚀 Project Workflow

## Phase 1 – Docker

- Created project directory
- Developed HTML application
- Created Dockerfile
- Built Docker Image (Version 1)
- Ran Docker Container
- Verified the application locally

---

## Phase 2 – Amazon ECR

- Created Amazon ECR Repository
- Logged in to Amazon ECR
- Tagged Docker Image
- Pushed Docker Image to Amazon ECR

---

## Phase 3 – Amazon EKS

- Created Amazon EKS Cluster
- Installed kubectl
- Connected kubectl to EKS
- Created Deployment
- Created ReplicaSet
- Created Pods
- Created Kubernetes Service

---

## Phase 4 – Application Deployment

- AWS automatically provisioned an Elastic Load Balancer
- Accessed the application using the ELB endpoint
- Verified Version 1 deployment

---

## Phase 5 – Rolling Update

- Modified the application to Version 2
- Built Docker Image (Version 2)
- Pushed Version 2 image to Amazon ECR
- Updated Kubernetes Deployment
- Kubernetes created a new ReplicaSet
- Old Pods were terminated automatically
- Version 2 deployed successfully without downtime

---

# 📂 Repository Structure

```
jags-shopping-devops-project

├── README.md

├── Docker
│   ├── Dockerfile
│   └── index.html

├── Kubernetes
│   ├── deployment.yaml
│   └── service.yaml

├── Documentation
│   └── MINI_PROJECT.docx

├── Screenshots

└── Architecture
```

---

# 📋 Kubernetes Objects Used

| Object | Purpose |
|---------|----------|
| Deployment | Manages application deployment |
| ReplicaSet | Maintains desired number of Pods |
| Pod | Runs the application |
| Service | Provides a stable endpoint |
| LoadBalancer | Exposes the application to the Internet |

---

# 🔄 Rolling Update Flow

```text
Version 1

↓

ReplicaSet V1

↓

Pods V1

↓

Deployment Updated

↓

ReplicaSet V2

↓

Pods V2

↓

Old Pods Removed

↓

Version 2 Running Successfully
```

---

# 📷 Project Screenshots

The Screenshots folder contains:

- Docker Image Build
- Docker Container
- Amazon ECR
- Amazon EKS Cluster
- Deployment
- Service
- Load Balancer
- Rolling Update
- Version 1 Output
- Version 2 Output

---

# 📚 Key Learning Outcomes

Through this project I gained practical experience in:

- Docker Image Creation
- Docker Container Deployment
- Amazon EC2
- Amazon ECR
- Amazon EKS
- Kubernetes Deployment
- ReplicaSets
- Pods
- Kubernetes Services
- AWS Elastic Load Balancer
- Rolling Update Strategy
- End-to-End DevOps Deployment

---

# 🚀 Future Enhancements

This project can be extended with:

- Jenkins CI/CD Pipeline
- GitHub Actions
- Helm Charts
- Ingress Controller
- ConfigMaps
- Kubernetes Secrets
- Horizontal Pod Autoscaler (HPA)
- Prometheus & Grafana Monitoring
- Centralized Logging
- Terraform

---

# 💡 Challenges Faced

During this project I learned how to troubleshoot and resolve:

- Docker installation issues
- ECR authentication errors
- kubectl configuration
- Kubernetes Deployment errors
- Incorrect image versions
- Service exposure
- Browser cache after Rolling Updates
- ReplicaSet updates

---

# 📖 Lessons Learned

This project helped me understand the complete DevOps workflow from application development to deployment on Kubernetes.

I gained practical knowledge of Docker, Amazon ECR, Amazon EKS, Kubernetes Deployments, Services, ReplicaSets, Pods, and Rolling Updates through hands-on implementation.

---

# 👨‍💻 Author

## Sai Kumar

Cloud Engineer

Currently learning:

- Docker
- Kubernetes
- AWS
- Terraform
- Jenkins
- DevOps

---

⭐ If you found this repository useful, please consider giving it a Star.
