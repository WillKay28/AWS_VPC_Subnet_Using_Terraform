# Docker_AWS_CI_CD_Pipeline
Docker AWS CI/CD Pipeline

In this project, I create EC2, Security Groups, and S3 infrastructure in AWS using Terraform (IaC) and use them to build a CI/CD pipeline for a containerized web app in Jenkins. I store the containerized image in Amazon ECR and deploy it Amazon ECS.  Note: server_key & server_key.pub -> These were SSH keys I generated using ssh-keygen to serve as keypairs for my servers.
