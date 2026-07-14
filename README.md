# 🛒 Jags Shopping – End-to-End DevOps Deployment on AWS

<p align="center">

![AWS](https://img.shields.io/badge/AWS-EKS-orange?style=for-the-badge&logo=amazonaws)
![Docker](https://img.shields.io/badge/Docker-Container-blue?style=for-the-badge&logo=docker)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-blue?style=for-the-badge&logo=kubernetes)
![Amazon ECR](https://img.shields.io/badge/Amazon-ECR-yellow?style=for-the-badge&logo=amazonaws)
![NGINX](https://img.shields.io/badge/WebServer-NGINX-green?style=for-the-badge&logo=nginx)

</p>

---

# 📖 Project Overview

This project demonstrates an **end-to-end deployment** of the **Jags Shopping** web application on **Amazon Web Services (AWS)**.

The application is containerized using **Docker**, stored securely in **Amazon Elastic Container Registry (Amazon ECR)**, deployed to **Amazon Elastic Kubernetes Service (Amazon EKS)**, and exposed to users using a **Kubernetes Service of type LoadBalancer**.

The project also demonstrates a **Rolling Update Deployment Strategy**, where the application is upgraded from **Version 1** to **Version 2** without downtime.

This project simulates a real-world DevOps deployment workflow from application development to deployment on Kubernetes.

---

# 🎯 Project Objectives

- Containerize the Jags Shopping web application using Docker.
- Store Docker images in Amazon Elastic Container Registry (Amazon ECR).
- Deploy the application to Amazon Elastic Kubernetes Service (Amazon EKS).
- Expose the application using a Kubernetes Service.
- Perform a Rolling Update from Version 1 to Version 2.
- Understand the complete DevOps deployment lifecycle on AWS.

---

# 🛠️ Technologies Used

| Category | Technology |
|-----------|------------|
| Cloud Provider | Amazon Web Services (AWS) |
| Compute | Amazon EC2 |
| Containerization | Docker |
| Container Registry | Amazon Elastic Container Registry (Amazon ECR) |
| Container Orchestration | Amazon Elastic Kubernetes Service (Amazon EKS) |
| Web Server | NGINX |
| Programming Language | HTML |
| Kubernetes Objects | Deployment, ReplicaSet, Pods, Service |
| Deployment Strategy | Rolling Update |
| CLI Tools | Docker CLI, AWS CLI, kubectl |

---

# 🏗️ Solution Architecture

```text
                    Developer
                        │
                        ▼
                Develop Jags Shopping
                        │
                        ▼
                  Docker Build
                        │
                        ▼
                  Docker Image
                        │
                        ▼
 Amazon Elastic Container Registry (ECR)
                        │
                        ▼
 Amazon Elastic Kubernetes Service (EKS)
                        │
                        ▼
            Kubernetes Deployment
                        │
                        ▼
                  ReplicaSet
                        │
                        ▼
                     Pods
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

- Created the project directory.
- Developed the Jags Shopping web application.
- Created the Dockerfile.
- Built Docker Image (Version 1).
- Created and tested the Docker container.

---

## Phase 2 – Amazon ECR

- Created an Amazon ECR repository.
- Logged in to Amazon ECR.
- Tagged the Docker image.
- Pushed Version 1 image to Amazon ECR.

---

## Phase 3 – Amazon EKS

- Created an Amazon EKS cluster.
- Installed kubectl.
- Connected kubectl to the EKS cluster.
- Created Kubernetes Deployment.
- Created ReplicaSet.
- Created Pods.
- Created Kubernetes Service.

---

## Phase 4 – Application Deployment

- AWS automatically provisioned an Elastic Load Balancer.
- Accessed the application using the ELB endpoint.
- Verified Version 1 deployment successfully.

---

## Phase 5 – Rolling Update

- Modified the application to Version 2.
- Built Docker Image (Version 2).
- Tagged and pushed Version 2 image to Amazon ECR.
- Updated the Kubernetes Deployment.
- Kubernetes automatically created a new ReplicaSet.
- Old Pods were terminated automatically.
- Version 2 was deployed successfully without downtime.

---

# 📂 Repository Structure

```text
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

| Kubernetes Object | Purpose |
|-------------------|----------|
| Deployment | Manages the application deployment |
| ReplicaSet | Maintains the desired number of Pods |
| Pod | Runs the application container |
| Service | Provides a stable endpoint to access the application |
| LoadBalancer | Exposes the application to external users |

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

- Project Setup
- Docker Build
- Docker Container
- Amazon ECR Repository
- Amazon EKS Cluster
- Kubernetes Deployment
- Kubernetes Service
- AWS Load Balancer
- Version 1 Output
- Version 2 Rolling Update

---

# 📚 Key Learning Outcomes

Through this project I gained hands-on experience with:

- Docker Image Creation
- Docker Container Deployment
- Amazon EC2
- Amazon Elastic Container Registry (Amazon ECR)
- Amazon Elastic Kubernetes Service (Amazon EKS)
- Kubernetes Deployments
- ReplicaSets
- Pods
- Kubernetes Services
- AWS Elastic Load Balancer
- Rolling Update Strategy
- End-to-End DevOps Deployment

---

# 💡 Challenges Faced

During this project I learned how to troubleshoot and resolve:

- Docker installation issues
- Amazon ECR authentication issues
- kubectl configuration
- Kubernetes Deployment errors
- Image version updates
- Service exposure
- Browser cache after Rolling Updates
- ReplicaSet updates

---

# 📖 Lessons Learned

This project helped me understand the complete DevOps deployment lifecycle by deploying the **Jags Shopping** web application using Docker, Amazon ECR, Amazon EKS, Kubernetes Deployments, ReplicaSets, Pods, Services, and the Rolling Update strategy.

---

# 🚀 Future Enhancements

In the next version of this project, I plan to implement:

- Jenkins CI/CD Pipeline
- GitHub Actions
- Helm Charts
- Kubernetes ConfigMaps
- Kubernetes Secrets
- Ingress Controller
- Horizontal Pod Autoscaler (HPA)
- Prometheus & Grafana Monitoring
- Centralized Logging
- Terraform

---

# 👨‍💻 Author

## Sai Kumar

Cloud Engineer

Currently learning:

- Docker
- Kubernetes
- Amazon Web Services (AWS)
- Terraform
- Jenkins
- DevOps

---

⭐ Thank you for visiting this repository.
