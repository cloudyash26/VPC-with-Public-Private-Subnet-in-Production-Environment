# VPC-with-Public-Private-Subnet-in-Production-Environment
## Overview
This project demonstrates the design and implementation of a VPC with public and private subnets across two availability zones, resulting in improved network security and scalability. The setup includes an Internet Gateway, NAT Gateways in both availability zones, route tables, and target groups for load balancers.

## Components
- VPC: Virtual Private Cloud with public and private subnets.
- Internet Gateway (IGW): Enables communication between the VPC and the internet.
- NAT Gateways: Allow instances in private subnets to initiate outbound traffic to the internet.
- Route Tables: Determine the routing of traffic within the VPC and between the VPC and the internet.
- Target Groups: Used with load balancers to route traffic to specific instances or IP addresses.
- Auto-Scaling Group: Launches and terminates servers in private subnets.
- Load Balancers: Route traffic from public subnets to private subnets.

## Architecture
- Public Subnets: Host load balancers and route traffic to private subnets.
- Private Subnets: Host instances launched by auto-scaling group.
- Availability Zones: Two zones for high availability and redundancy.

## Outcomes
- Improved Network Security: Private subnets are isolated from the internet.
- Scalability: Auto-scaling group launches and terminates instances based on demand.
- High Availability: Load balancers and auto-scaling group ensure application availability.
- Cost Optimization: NAT gateways and auto-scaling group reduce costs.

## Technologies Used
- AWS: VPC, EC2 (Jump Server), Auto Scaling Groups, Load Balancer, Target Groups, NAT Gateway, Nacl, Security Groups, Internet Gateway, Route Tables, SSH

## For a detailed walkthrough of the project, including implementation steps and lessons learned, visit my Hashnode blog post: https://hashnode.com/@yashparab45


