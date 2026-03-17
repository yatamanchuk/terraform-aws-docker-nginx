# AWS Terraform DevOps Project

## Overview
This project demonstrates Infrastructure as Code (IaC) by provisioning AWS infrastructure using 
Terraform and automatically deploying a containerized web application using Docker.

## Features
- Automated EC2 provisioning using Terraform
- Security group configuration (SSH + HTTP access)
- Docker installation via user-data script
- Nginx container deployment
- Public web server accessible via EC2 public IP

## Architecture
Terraform → AWS → EC2 → Docker → Nginx

## Technologies Used
- AWS (EC2, Security Groups)
- Terraform
- Docker
- Linux

## Deployment Steps
### 1. Configure AWS CLI
Make sure AWS CLI is installed and configured with your credentials:

```bash

### 2. Initialize Terraform
terraform init


### 3. Review Execution Plan
terraform plan

### 4. Deploy Infrastructure
terraform apply
Type yes when prompted.

### 5. Access Application
Open in browser: http://<EC2-PUBLIC-IP>

###6. Destroy Resources (Cleanup)
terraform destroy

## Expected Output
Nginx welcome page running from a Docker container on AWS EC2.

## Key Learning Outcomes
- Infrastructure as Code with Terraform
- Cloud resource provisioning in AWS
- Containerized deployments using Docker
- Automated server configuration with user-data scripts

## Future Improvements
- Add CI/CD pipeline (GitHub Actions)
- Deploy custom application instead of Nginx
- Add monitoring (Prometheus + Grafana)
- Use Terraform modules for scalability

## Author
Yaroslav Atamanchuk
