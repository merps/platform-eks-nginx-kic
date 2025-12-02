# Platform EKS + NGINX KIC

This repository demonstrates a production-grade EKS platform using:

- AWS EKS (terraform-aws-eks)
- NGINX Kubernetes Ingress Controller (KIC)
- IRSA-enabled controllers
- Calico networking (optional)
- Sample workloads (Juice Shop, demo service)
- GitHub Actions CI for Terraform & K8s linting

## Architecture Diagram

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/merps/merps/assets/diagrams/eks-platform-blueprint-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/merps/merps/blob/main/assets/diagrams/eks-platform-blueprint-light.svg">
  <img alt="EKS + NGINX KIC Architecture" src="https://github.com/merps/merps/assets/diagrams/eks-platform-blueprint-light.svg">
</picture>

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