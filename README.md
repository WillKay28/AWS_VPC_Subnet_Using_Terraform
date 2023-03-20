# AWS_VPC_Subnet_Using_Terraform

In this project, I create EC2 Instances, Security Groups, VPC, Subnets, Route table, Internet Gateway and S3 infrastructure in AWS using Terraform (IaC).

In summary, I use Terraform to: 

1. Create a VPC in a region and
2. Create public & private subnets and cidr blocks in the VPC in different Availability Zones
3. Create a route table of the IP addresses of the subnets
4. Connect the Route Table to Internet Gateway
5. Create security group rules for inbound (ingress) & outbound (egress) traffic to the VPC
6. Create the necessary EC2 Instances in the subnets and attach extra EBS volume.
7. Output the Public IP addresses of the servers. 

Note: 
1. dove_key & dove_key.pub -> These are SSH keys I generate using ssh-keygen to serve as keypairs for my instance.
2. backend.tf stores the state files of the resources in s3 bucket.
3. web.sh is used to provision the EC2 Instance.

