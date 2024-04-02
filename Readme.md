# Django Blog CloudFormation Project
This CloudFormation project is designed to set up a scalable infrastructure for a Django-based blog application on AWS. The infrastructure includes VPC setup, RDS for database management, S3 buckets for media storage, DynamoDB for NoSQL data storage, an Elastic Load Balancer for traffic distribution, Auto Scaling for handling varying traffic loads, IAM roles and permissions for security, Lambda functions for event-driven actions, CloudFront distribution for content delivery, and Route 53 for DNS management.

# Project Structure
# The project is structured as follows:

**VPC & Subnet Configurations:** Defines the Virtual Private Cloud (VPC) along with public and private subnets across multiple availability zones.

**Security Group Configurations:** Sets up security groups to control inbound and outbound traffic to various resources such as EC2 instances, RDS, and NAT gateway.

**RDS, S3, and DynamoDB Configurations:** Configures RDS for database management, S3 buckets for media storage, and DynamoDB for NoSQL data storage.

**NAT Configurations:** Sets up a NAT instance for outbound internet access from private subnets.

**IAM Configurations:** Defines IAM roles and policies for granting permissions to EC2 instances and Lambda functions.

**Launch Template Configurations:** Creates a launch template for EC2 instances with user data to bootstrap the application environment.

**Load Balancer Configurations:** Configures an Elastic Load Balancer (ELB) for distributing incoming traffic across EC2 instances.

**Auto Scaling Configurations:** Sets up Auto Scaling to automatically adjust the number of EC2 instances based on traffic demand.

**CloudFront & Route 53 Configurations:** Configures CloudFront distribution for content delivery and Route 53 for DNS routing.

**Lambda Configurations:** Defines Lambda functions for event-driven actions such as logging file uploads to DynamoDB.
