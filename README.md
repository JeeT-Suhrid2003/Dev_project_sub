# Full-Stack Blogging App — CI/CD Demonstration

A complete CI/CD example that builds, tests, and deploys a full-stack blogging application using Jenkins, Docker, Nexus, Terraform, and Kubernetes, with monitoring via Prometheus and Grafana.

---

## Table of contents
- Project overview
- Key features
- Tech stack
- Repository structure
- Quick start
- CI/CD pipeline (high level)
- Deployment & infrastructure
- Monitoring & observability
- Contributing
- License

---

## Project overview
This repository demonstrates a production-oriented CI/CD pipeline for a full-stack blogging application. It includes scripts and manifests for building images, running static analysis, storing artifacts, provisioning infrastructure (EKS) with Terraform, deploying to Kubernetes, and monitoring with Prometheus and Grafana.

The goal is to provide a repeatable, automated workflow suitable for a course submission or a reference implementation for learning modern DevOps practices.

---

## Key features
- Automated build, test, and deployment pipeline (Jenkins)
- Static code analysis (SonarQube) and vulnerability scanning (Trivy)
- Containerization (Docker) and artifact management (Nexus / DockerHub)
- Infrastructure as Code (Terraform) for AWS EKS
- Kubernetes manifests for app deployment, RBAC, and services
- Monitoring stack: Prometheus, Grafana, and Blackbox Exporter

---

## Tech stack
- CI: Jenkins  
- Code quality: SonarQube  
- Artifact repository: Nexus / DockerHub  
- Container runtime: Docker  
- Orchestration: Kubernetes (EKS)  
- IaC: Terraform  
- Monitoring: Prometheus, Grafana, Blackbox Exporter  
- Security scanning: Trivy

---

## Repository structure
```text
/full-stack-blogging-app
├── /ci-scripts
│   ├── install_jenkins.sh
│   ├── install_docker.sh
│   ├── install_blackbox.sh
│   ├── prometheus.yml
│   └── grafana_dashboard.json
├── /kubernetes
│   ├── deployment.yml
│   ├── service.yml
│   ├── role.yaml
│   ├── rolebinding.yaml
│   └── serviceaccount.yaml
├── /terraform
│   ├── main.tf
│   ├── variables.tf
│   └── outputs.tf
├── /src
│   ├── app.js
│   ├── Dockerfile
│   └── ...
└── README.md
```
---
[!imge.png]
