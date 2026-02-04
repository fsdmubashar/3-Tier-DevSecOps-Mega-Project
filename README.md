# 🚀 3-Tier DevSecOps Mega Project

<div align="center">

![DevSecOps](https://img.shields.io/badge/DevSecOps-Enabled-brightgreen?style=for-the-badge)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)

**A Production-Ready, Security-First, Cloud-Native Application Deployment Pipeline**

[Documentation](#-documentation) • [Architecture](#-architecture) • [Getting Started](#-getting-started) • [Features](#-features) • [Contributing](#-contributing)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Architecture](#-architecture)
- [Key Features](#-key-features)
- [Technology Stack](#-technology-stack)
- [Prerequisites](#-prerequisites)
- [Getting Started](#-getting-started)
- [Project Structure](#-project-structure)
- [CI/CD Pipeline](#-cicd-pipeline)
- [Security Implementation](#-security-implementation)
- [Monitoring & Observability](#-monitoring--observability)
- [Deployment Guide](#-deployment-guide)
- [Troubleshooting](#-troubleshooting)
- [Best Practices](#-best-practices)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 🌟 Overview

This project demonstrates a **complete end-to-end DevSecOps implementation** for a 3-tier web application with integrated security scanning, automated CI/CD pipelines, infrastructure as code, and comprehensive monitoring solutions.

### 🎯 Project Objectives

- ✅ Implement a **security-first** approach to application deployment
- ✅ Automate **infrastructure provisioning** using Terraform
- ✅ Build a **robust CI/CD pipeline** with Jenkins
- ✅ Deploy on **Kubernetes** with high availability
- ✅ Integrate **comprehensive security scanning** at every stage
- ✅ Set up **monitoring and alerting** with Prometheus & Grafana
- ✅ Follow **DevSecOps best practices** throughout

---

## 🏗️ Architecture

### 3-Tier Application Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                     PRESENTATION LAYER                       │
│  ┌──────────────────────────────────────────────────────┐  │
│  │         Frontend (React/Angular/Vue.js)               │  │
│  │         - User Interface                              │  │
│  │         - Client-side Logic                           │  │
│  └──────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                      APPLICATION LAYER                       │
│  ┌──────────────────────────────────────────────────────┐  │
│  │         Backend API (Node.js/Java/Python)             │  │
│  │         - Business Logic                              │  │
│  │         - API Endpoints                               │  │
│  │         - Authentication & Authorization              │  │
│  └──────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                        DATA LAYER                            │
│  ┌──────────────────────────────────────────────────────┐  │
│  │         Database (PostgreSQL/MongoDB/MySQL)           │  │
│  │         - Data Storage                                │  │
│  │         - Data Management                             │  │
│  └──────────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────────┘
```

### DevSecOps Pipeline Architecture

```
┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
│   SCM    │───▶│  Build   │───▶│   Test   │───▶│  Scan    │
│  GitHub  │    │ Jenkins  │    │  Unit    │    │ Security │
└──────────┘    └──────────┘    └──────────┘    └──────────┘
                                                       │
                                                       ▼
┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
│ Monitor  │◀───│  Deploy  │◀───│ Package  │◀───│ Quality  │
│Prometheus│    │Kubernetes│    │  Docker  │    │ SonarQube│
└──────────┘    └──────────┘    └──────────┘    └──────────┘
```

---

## ✨ Key Features

### 🔐 Security First

- **SAST (Static Application Security Testing)** with SonarQube
- **DAST (Dynamic Application Security Testing)** with OWASP ZAP
- **Container Scanning** with Trivy
- **Dependency Scanning** with OWASP Dependency Check
- **Secret Scanning** to prevent credential leaks
- **Security Policies** as Code

### 🔄 Automated CI/CD

- **Continuous Integration** with Jenkins
- **Automated Testing** (Unit, Integration, E2E)
- **Build Automation** with Docker
- **Continuous Deployment** to Kubernetes
- **GitOps** workflow implementation
- **Rollback Mechanisms**

### ☁️ Cloud Native

- **Kubernetes** orchestration
- **Containerized** applications
- **Microservices** architecture support
- **Auto-scaling** capabilities
- **High Availability** design
- **Cloud Provider** agnostic (AWS/Azure/GCP)

### 📊 Monitoring & Observability

- **Metrics Collection** with Prometheus
- **Visualization** with Grafana dashboards
- **Logging** with ELK Stack
- **Distributed Tracing** with Jaeger
- **Alerting** configuration
- **Health Checks** and Probes

---

## 🛠️ Technology Stack

### Infrastructure & Orchestration

| Technology | Purpose | Version |
|------------|---------|---------|
| Kubernetes | Container Orchestration | 1.28+ |
| Docker | Containerization | 24.0+ |
| Terraform | Infrastructure as Code | 1.5+ |
| Helm | Kubernetes Package Manager | 3.12+ |
| AWS/Azure/GCP | Cloud Provider | Latest |

### CI/CD & Automation

| Technology | Purpose | Version |
|------------|---------|---------|
| Jenkins | CI/CD Server | 2.400+ |
| GitHub Actions | CI/CD Alternative | N/A |
| ArgoCD | GitOps Operator | 2.8+ |
| Ansible | Configuration Management | 2.15+ |

### Security Tools

| Technology | Purpose | Version |
|------------|---------|---------|
| SonarQube | Code Quality & SAST | 9.9+ |
| Trivy | Container Scanning | Latest |
| OWASP ZAP | DAST | 2.14+ |
| HashiCorp Vault | Secrets Management | 1.15+ |
| Falco | Runtime Security | Latest |

### Monitoring & Logging

| Technology | Purpose | Version |
|------------|---------|---------|
| Prometheus | Metrics Collection | 2.45+ |
| Grafana | Visualization | 10.0+ |
| ELK Stack | Logging | 8.9+ |
| Jaeger | Distributed Tracing | 1.47+ |

---

## 📦 Prerequisites

### Required Software

```bash
# Docker
Docker version 24.0.0 or higher

# Kubernetes
kubectl version 1.28.0 or higher
minikube/kind/EKS/AKS/GKE

# Terraform
Terraform v1.5.0 or higher

# Jenkins
Jenkins 2.400 or higher

# Other Tools
- Git 2.40+
- Helm 3.12+
- AWS CLI / Azure CLI / gcloud CLI
- jq (for JSON processing)
```

### Required Accounts

- ✅ GitHub Account
- ✅ Docker Hub Account
- ✅ AWS/Azure/GCP Account (based on cloud provider choice)
- ✅ SonarCloud Account (or self-hosted SonarQube)

### System Requirements

```
Minimum:
- CPU: 4 cores
- RAM: 8 GB
- Storage: 50 GB

Recommended:
- CPU: 8 cores
- RAM: 16 GB
- Storage: 100 GB
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/fsdmubashar/3-Tier-DevSecOps-Mega-Project.git
cd 3-Tier-DevSecOps-Mega-Project
```

### 2️⃣ Setup Environment Variables

```bash
# Copy environment template
cp .env.example .env

# Edit with your configurations
nano .env
```

Required Environment Variables:
```bash
# AWS Configuration
AWS_ACCESS_KEY_ID=your_access_key
AWS_SECRET_ACCESS_KEY=your_secret_key
AWS_REGION=us-east-1

# Docker Hub
DOCKER_USERNAME=your_username
DOCKER_PASSWORD=your_password

# SonarQube
SONAR_HOST_URL=https://sonarcloud.io
SONAR_TOKEN=your_sonar_token

# Database
DB_HOST=database_host
DB_PORT=5432
DB_NAME=your_database
DB_USER=your_user
DB_PASSWORD=your_password
```

### 3️⃣ Infrastructure Setup

```bash
# Navigate to Terraform directory
cd terraform

# Initialize Terraform
terraform init

# Plan infrastructure changes
terraform plan

# Apply infrastructure
terraform apply -auto-approve
```

### 4️⃣ Deploy Application

```bash
# Build Docker images
docker-compose build

# Push to Docker Hub
docker-compose push

# Deploy to Kubernetes
kubectl apply -f k8s/

# Verify deployment
kubectl get pods -n production
```

### 5️⃣ Setup Jenkins Pipeline

```bash
# Install Jenkins plugins
- Docker Pipeline
- Kubernetes
- SonarQube Scanner
- OWASP Dependency-Check
- Terraform

# Configure Jenkins credentials
- GitHub credentials
- Docker Hub credentials
- AWS credentials
- SonarQube token

# Create Jenkins pipeline job
- Use Jenkinsfile from repository
- Configure webhook for automatic triggers
```

---

## 📁 Project Structure

```
3-Tier-DevSecOps-Mega-Project/
│
├── .github/
│   └── workflows/              # GitHub Actions workflows
│
├── frontend/                   # Frontend application
│   ├── src/
│   ├── public/
│   ├── Dockerfile
│   └── package.json
│
├── backend/                    # Backend API
│   ├── src/
│   ├── tests/
│   ├── Dockerfile
│   └── requirements.txt
│
├── database/                   # Database scripts
│   ├── migrations/
│   ├── seeds/
│   └── init.sql
│
├── terraform/                  # Infrastructure as Code
│   ├── modules/
│   ├── environments/
│   ├── main.tf
│   └── variables.tf
│
├── k8s/                       # Kubernetes manifests
│   ├── deployments/
│   ├── services/
│   ├── ingress/
│   ├── configmaps/
│   └── secrets/
│
├── jenkins/                   # Jenkins configuration
│   ├── Jenkinsfile
│   └── shared-library/
│
├── monitoring/                # Monitoring configuration
│   ├── prometheus/
│   ├── grafana/
│   └── alertmanager/
│
├── scripts/                   # Utility scripts
│   ├── setup.sh
│   ├── deploy.sh
│   └── cleanup.sh
│
├── docs/                      # Documentation
│   ├── architecture.md
│   ├── deployment.md
│   └── troubleshooting.md
│
├── docker-compose.yml         # Local development
├── .env.example              # Environment template
└── README.md                 # This file
```

---

## 🔄 CI/CD Pipeline

### Pipeline Stages

```yaml
1. Code Checkout
   └── Pull latest code from GitHub

2. Build
   ├── Compile application
   ├── Run linters
   └── Static code analysis

3. Test
   ├── Unit tests
   ├── Integration tests
   └── Code coverage report

4. Security Scan
   ├── SAST (SonarQube)
   ├── Dependency Check (OWASP)
   ├── Secret Scanning
   └── Container Scanning (Trivy)

5. Build Docker Image
   ├── Create optimized image
   ├── Tag with version
   └── Scan image for vulnerabilities

6. Push to Registry
   └── Push to Docker Hub/ECR

7. Deploy to Dev
   ├── Apply Kubernetes manifests
   ├── Run smoke tests
   └── Health checks

8. Integration Tests
   └── Run E2E tests in dev environment

9. Deploy to Staging
   ├── Promote to staging
   └── Run performance tests

10. Manual Approval
    └── Wait for approval

11. Deploy to Production
    ├── Blue-Green deployment
    ├── Monitor metrics
    └── Automatic rollback if issues
```

### Jenkinsfile Example

```groovy
pipeline {
    agent any
    
    environment {
        DOCKER_REGISTRY = 'docker.io'
        DOCKER_IMAGE = 'fsdmubashar/3tier-app'
        KUBECONFIG = credentials('kubeconfig')
    }
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                sh 'docker build -t ${DOCKER_IMAGE}:${BUILD_NUMBER} .'
            }
        }
        
        stage('Security Scan') {
            parallel {
                stage('SonarQube') {
                    steps {
                        withSonarQubeEnv('SonarQube') {
                            sh 'mvn sonar:sonar'
                        }
                    }
                }
                stage('Trivy Scan') {
                    steps {
                        sh 'trivy image ${DOCKER_IMAGE}:${BUILD_NUMBER}'
                    }
                }
            }
        }
        
        stage('Push Image') {
            steps {
                sh 'docker push ${DOCKER_IMAGE}:${BUILD_NUMBER}'
            }
        }
        
        stage('Deploy to Kubernetes') {
            steps {
                sh '''
                    kubectl set image deployment/app \
                    app=${DOCKER_IMAGE}:${BUILD_NUMBER} \
                    -n production
                '''
            }
        }
    }
    
    post {
        always {
            cleanWs()
        }
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
```

---

## 🔐 Security Implementation

### Security Scanning Tools

1. **SonarQube (SAST)**
   - Code quality analysis
   - Security vulnerability detection
   - Code smell identification
   - Technical debt tracking

2. **Trivy (Container Scanning)**
   - OS package vulnerabilities
   - Application dependency vulnerabilities
   - IaC misconfigurations
   - Secret detection

3. **OWASP Dependency Check**
   - Known vulnerable dependencies
   - CVE database matching
   - License analysis

4. **OWASP ZAP (DAST)**
   - Dynamic security testing
   - Penetration testing
   - API security testing

### Security Best Practices Implemented

- ✅ Non-root container users
- ✅ Read-only root filesystems
- ✅ Resource limits and quotas
- ✅ Network policies
- ✅ Pod security policies
- ✅ Secrets encryption
- ✅ RBAC implementation
- ✅ Security contexts
- ✅ Image signing
- ✅ Vulnerability scanning

---

## 📊 Monitoring & Observability

### Prometheus Metrics

```yaml
# Application Metrics
- http_requests_total
- http_request_duration_seconds
- http_response_size_bytes
- application_errors_total

# Infrastructure Metrics
- node_cpu_usage
- node_memory_usage
- pod_cpu_usage
- pod_memory_usage

# Custom Business Metrics
- user_registrations_total
- orders_processed_total
- payment_success_rate
```

### Grafana Dashboards

1. **Application Performance**
   - Request rate
   - Error rate
   - Response time
   - Throughput

2. **Infrastructure Health**
   - CPU usage
   - Memory usage
   - Disk I/O
   - Network traffic

3. **Business Metrics**
   - User activity
   - Transaction volume
   - Revenue metrics

---

## 📖 Deployment Guide

### Development Environment

```bash
# Start local development
docker-compose up -d

# Access application
http://localhost:3000  # Frontend
http://localhost:8080  # Backend API
http://localhost:5432  # PostgreSQL
```

### Staging Environment

```bash
# Deploy to staging
kubectl apply -f k8s/staging/

# Verify deployment
kubectl get pods -n staging

# Run tests
./scripts/test-staging.sh
```

### Production Environment

```bash
# Deploy to production (with approval)
kubectl apply -f k8s/production/

# Monitor deployment
kubectl rollout status deployment/app -n production

# Verify health
curl https://api.yourdomain.com/health
```

---

## 🐛 Troubleshooting

### Common Issues

#### Issue 1: Pod CrashLoopBackOff

```bash
# Check pod logs
kubectl logs <pod-name> -n production

# Describe pod
kubectl describe pod <pod-name> -n production

# Common causes:
- Incorrect environment variables
- Database connection issues
- Resource limits too low
```

#### Issue 2: ImagePullBackOff

```bash
# Check image exists
docker pull <image-name>

# Verify credentials
kubectl get secret docker-registry-secret -o yaml

# Solution:
kubectl create secret docker-registry docker-registry-secret \
  --docker-server=docker.io \
  --docker-username=<username> \
  --docker-password=<password>
```

#### Issue 3: Service Not Accessible

```bash
# Check service
kubectl get svc -n production

# Check endpoints
kubectl get endpoints -n production

# Check ingress
kubectl get ingress -n production
```

---

## 💡 Best Practices

### 1. Code Quality
- Write clean, maintainable code
- Follow coding standards
- Implement comprehensive tests
- Use code reviews

### 2. Security
- Regular security audits
- Keep dependencies updated
- Use secrets management
- Implement least privilege

### 3. Operations
- Implement proper monitoring
- Set up alerting
- Document everything
- Plan for disaster recovery

### 4. CI/CD
- Keep pipelines fast
- Fail fast, fail early
- Automate everything
- Version everything

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Contribution Guidelines

- Follow the existing code style
- Write meaningful commit messages
- Add tests for new features
- Update documentation
- Keep PRs focused and small

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📞 Contact

**Muhammad Mubashar Karamat**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/mubashar-karamat-833457245/)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:city.mubashar@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/fsdmubashar)
[![Medium](https://img.shields.io/badge/Medium-Follow-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@city.mubashar)

---

## 🙏 Acknowledgments

- Thanks to the open-source community
- Inspired by industry best practices
- Built with modern DevSecOps tools

---

## 📚 Additional Resources

- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [Docker Documentation](https://docs.docker.com/)
- [Jenkins Documentation](https://www.jenkins.io/doc/)
- [Terraform Documentation](https://www.terraform.io/docs/)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [12 Factor App](https://12factor.net/)

---

<div align="center">

**⭐ If you find this project helpful, please give it a star!**

**Made with ❤️ by [Muhammad Mubashar Karamat](https://github.com/fsdmubashar)**

![Visitors](https://komarev.com/ghpvc/?username=fsdmubashar-3tier&color=brightgreen&style=for-the-badge)

</div>
