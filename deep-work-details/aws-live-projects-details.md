# AWS Live Projects

AWS projects should be performed both using AWS Console (*ClickOps*) and Terraform (*Infrastructure as Code IaC*)

1. Create a VPC with 
  - us-east-1 Region and us-east-1a AZ
  - 1 Public subnet 
  - 1 Route Table for the subnet
  - 1 Internet Gateway
  - 1 EC2 Instance using Ubuntu 24.04 AMI
  - 1 Security Group
2. Create a VPC with 
  - us-east-1 Region and us-east-1a AZ
  - 1 Public subnet and 2 Private Subnets
  - 3 Route Table for each of the subnets
  - 1 Internet Gateway
  - 1 NAT Gateway for the EC2 instances in the two Private subnets
  - 1 EC2 Instance using Ubuntu 24.04 AMI in each of the subnets
  - 1 Security Group per EC2 instance
3. Use the setup in 2 above as base and
  - Setup nginx as a web server on public subnet with SSL termination
4. Use the setup in 2 above as base and
  - Setup nginx as reverse proxy (layer 7) on public subnet with SSL termination
  - Setup nginx as Web Server (HTTP only) on any one of the private subnet 
5. Use the setup in 2 above as base and
  - Setup nginx as reverse proxy (layer 7) and load balancer on public subnet with SSL termination
  - Setup multiple nginx as Web Servers (HTTP only) on any one of the private subnet 
6. Use the setup in 2 above as base and
  - Setup nginx as reverse proxy (layer 4) on public subnet
  - Setup nginx as Web Server (HTTP only) on any one of the private subnet 
7. Use the setup in 2 above as base and
  - Setup nginx as reverse proxy (layer 4) and load balancer on public subnet
  - Setup multiple nginx as Web Servers (HTTP only) on any one of the private subnet