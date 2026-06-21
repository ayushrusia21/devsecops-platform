# DevSecOps Platform

## Architecture

```text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions CI/CD
    ├── Helm Lint
    ├── Docker Build
    ├── Trivy Scan
    └── Docker Push
    │
    ▼
Docker Hub
    │
    ▼
ArgoCD (GitOps)
    │
    ▼
Kubernetes Cluster (Kind / EKS)
    │
    ├── User Service Deployment
    ├── Service
    ├── Ingress
    ├── HPA
    ├── Network Policies
    ├── Istio Service Mesh
    │     ├── Envoy Sidecar
    │     └── mTLS (STRICT)
    │
    ├── Vault
    │     └── Secrets Management
    │
    ├── Prometheus
    ├── Grafana
    └── Falco Runtime Security
```

## Features

* Kubernetes Deployment & Service Management
* Helm-based Application Packaging
* GitHub Actions CI/CD Pipeline
* Docker Hub Image Registry
* Trivy Container Security Scanning
* ArgoCD GitOps Deployment
* Prometheus Monitoring
* Grafana Dashboards
* HashiCorp Vault Secret Management
* Falco Runtime Security Monitoring
* Istio Service Mesh
* Mutual TLS (mTLS)
* Horizontal Pod Autoscaling (HPA)
* Network Policies
* Pod Disruption Budgets

```
```

