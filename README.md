## Project Name
InfraSync

## Description

This project is an infrastructure provisioning project using Terraform and AWS. It automates the deployment of a VPC infrastructure on AWS, including the creation of VPC, subnets, internet gateway, NAT gateway, route tables, and related resources. The project utilizes GitHub Actions for automating the deployment process.

## Features

- Infrastructure as Code: The project leverages Terraform to define and manage the infrastructure resources in a declarative and version-controlled manner.
- VPC Provisioning: The project provisions a VPC infrastructure with public and private subnets spread across multiple availability zones.
- High Availability: The infrastructure is designed to be highly available by distributing resources across different availability zones.
- Automated Deployment: GitHub Actions is used to automate the deployment process, making it easier to maintain and manage the infrastructure.

## Technologies Used

- Terraform: Infrastructure provisioning tool used to define and manage AWS resources.
- AWS (Amazon Web Services): Cloud platform where the infrastructure is provisioned.
- GitHub Actions: CI/CD platform used for automating the deployment process.
- Amazon VPC: Virtual Private Cloud for networking isolation.
- Subnets: Divided network segments for organizing resources.
- Internet Gateway: Enables communication between VPC and the internet.
- NAT Gateway: Provides outbound internet access for resources in private subnets.
- Route Tables: Define routing rules for network traffic.
- S3 Bucket: Storage for Terraform state file and versioning.
- DynamoDB Table: Locking mechanism for Terraform state file.

## Requirements

- AWS Account: Access to an AWS account to provision the infrastructure resources.
- AWS Credentials: Valid AWS access key ID and secret access key with appropriate permissions.
- Terraform: Installed Terraform CLI version 0.13.0 or higher on your local machine.
- GitHub Repository: A GitHub repository to store the project code and utilize GitHub Actions.

Ensure that the AWS credentials are securely stored and properly configured in the environment or as GitHub secrets.
