# Golden Owl DevOps Internship - Technical Test
Submitted by: Nguyen Gia Bao (GiaBao1006)

## Your Mission 🌟
Your mission, should you choose to accept it, is to craft a CI job that:
1. Forks this repository to your personal GitHub account.
2. Dockerizes a Node.js application.
3. Establishes an automated CI/CD build process using GitHub Actions workflow and a container registry service such as DockerHub or Amazon Elastic Container Registry (ECR) or similar services.
4. Initiates CI tests automatically when changes are pushed to the feature branch on GitHub.
5. Utilizes GitHub Actions for Continuous Deployment (CD) to deploy the application to major cloud providers like AWS EC2, AWS ECS or Google Cloud (please submit the deployment link).

## Tech Stack
1. Cloud: AWS (Amazon Web Services)
        Compute: EC2 (Elastic Compute Cloud)
        Networking: VPC, Subnets, Route Tables, Internet Gateway, ALB
        Scaling & HA: Auto Scaling Group (ASG)
        Container Registry: ECR (Elastic Container Registry)

2. Infrastructure as Code: Terraform

3. Containerization: Docker

4. CI/CD: GitHub Actions

5. Application: Node.js

## Architecture Diagram



## How To Deploy
Prerequisites:
    Terraform CLI installed.
    AWS CLI installed and configured.
    Docker installed and running.

1. Terraform:
cd terraform #Move to folder Terra
terraform init #Initialize Terraform in the current directory
terraform plan #Generate and show an execution plan
terraform apply #Apply the changes

2. Docker:
cd .. #Move to folder root
aws ecr get-login-password --region [REGION] | docker login --username AWS --password-stdin [ACCOUNT_ID].dkr.ecr.[REGION].amazonaws.com #Log in to AWS ECR
docker buildx build --platform linux/amd64 -t [ECR_REPOSITORY_URL]:latest . #Build the Docker image (M1 platform)
docker push [ECR_REPOSITORY_URL]:latest #Push the image to ECR

3. GitHub CI/CD Pipeline:
Using GitHub Actions
    CI (Continuous Integration): Automatically runs npm test on every Pull Request.
    CD (Continuous Deployment): Automatically builds, pushes, and deploys the application with zero-downtime on every merge to the master branch.

# Important
Create new user in IAM console, then create Access key and Secret Key to put in GitHub Actions. It's use for CD.

## Clean all
terraform destroy #Destroy the Terraform-managed infrastructure