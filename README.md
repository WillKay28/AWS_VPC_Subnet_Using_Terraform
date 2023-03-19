# Docker_AWS_CI_CD_Pipeline
Docker AWS CI/CD Pipeline

In this project, I create EC2 Instances, Security Groups, VPC, Subnets, Route table, Internet Gateway and S3 infrastructure in AWS using Terraform (IaC) and use them to build a CI/CD pipeline for a containerized web app in Jenkins. 

In summary, I use Terraform to: 

1. Create a VPC in a region and
2. Create public & private subnets and cidr blocks in the VPC in different Availability Zones
3. Create a route table of the IP addresses of the subnets
4. Connect the Route Table to Internet Gateway
5. Create security group rules for inbound (ingress) & outbound (egress) traffic to the VPC
6. Create the necessary EC2 Instances in the subnets and attach extra EBS volume.
7. Output the Public IP addresses of the servers. 

I store the containerized image in Amazon ECR and deploy it Amazon ECS.  Note: server_key & server_key.pub -> These were SSH keys I generated using ssh-keygen to serve as keypairs for my servers.
