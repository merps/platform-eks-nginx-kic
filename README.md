# Platform EKS + NGINX KIC

This repository demonstrates a production-grade EKS platform using:

- AWS EKS (terraform-aws-eks)
- NGINX Kubernetes Ingress Controller (KIC)
- IRSA-enabled controllers
- Calico networking (optional)
- Sample workloads (Juice Shop, demo service)
- GitHub Actions CI for Terraform & K8s linting

## Architecture Diagram
(see docs/architecture-diagram.png)

## Key Features
- Modular Terraform
- Secure IRSA permissions
- TLS termination
- L7 routing
- Observability hooks

## Usage

```
terraform init
terraform apply -var-file="env/dev.tfvars"
```