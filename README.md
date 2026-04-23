# AWS-K8s-CICD-Project

## Architecture
- Frontend: React app served via Nginx
- Backend: .NET API
- Database: MySQL RDS
- Container Registry: Amazon ECR
- Orchestration: Amazon EKS
- CI/CD: GitHub Actions

## Pipeline
- CI: Lint, Test, Build, Security Scan, Push to ECR
- CD Staging: Auto-deploy on trigger
- CD Production: Manual approval required

## Environments
- Staging: stg.eks-project.com (1 replica)
- Production: eks-project.com (3 replicas)
