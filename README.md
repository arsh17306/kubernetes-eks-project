# Kubernetes End-to-End Project on AWS EKS

## Overview
This project demonstrates deployment of a containerized application on Amazon EKS (Elastic Kubernetes Service) using Kubernetes manifests and Docker.

The project covers:
- EKS cluster setup
- Kubernetes deployments
- Services and networking
- Containerized application deployment
- Pod and service management

---

## AWS Services Used

- Amazon EKS
- Amazon EC2
- Amazon VPC
- IAM
- Elastic Load Balancer (ELB)

---

## Tools & Technologies

- Kubernetes
- Docker
- kubectl
- eksctl
- Git & GitHub
- VS Code

---

## Project Structure

```text
kubernetes-eks-project/
│
├── README.md
├── screenshots/
├── kubernetes-manifests/
│   ├── deployment.yaml
│   ├── service.yaml
│   └── ingress.yaml
│
└── app/
```

---

## Steps Performed

### 1. Created EKS Cluster
```bash
eksctl create cluster
```

### 2. Configured kubectl
```bash
aws eks update-kubeconfig --region us-east-1 --name my-cluster
```

### 3. Created Kubernetes Deployment
```bash
kubectl apply -f deployment.yaml
```

### 4. Created Kubernetes Service
```bash
kubectl apply -f service.yaml
```

### 5. Verified Pods and Services
```bash
kubectl get pods
kubectl get svc
```

---

## Kubernetes Components Used

### Deployment
Used to manage application pods and replicas.

### Service
Used to expose the application externally.

### Pods
Running containers inside Kubernetes cluster.

---

## Screenshots

### EKS Cluster
![Cluster](screenshots/eks-cluster.png)

### Worker Nodes
![Nodes](screenshots/nodes.png)

### Running Pods
![Pods](screenshots/deployment.png)

### Kubernetes Service
![Service](screenshots/service.png)

### Application Running
![Application](screenshots/app-running.png)

---

## Outcome

Successfully deployed and managed a containerized application on AWS EKS using Kubernetes.

The project demonstrates:
- Kubernetes orchestration
- EKS cluster management
- Container deployment
- Service exposure
- Cloud-native deployment workflow

---

## Author

Arsh
