## Project Name
InfraSync

## Description

This project is an infrastructure provisioning project using Terraform and AWS. It automates the deployment of a VPC infrastructure on AWS, including the creation of VPC, subnets, internet gateway, NAT gateway, route tables, and related resources. The project utilizes GitHub Actions for automating the deployment process.

## Features

- Infrastructure as Code: The project leverages Terraform to define and manage the infrastructure resources in a declarative and version-controlled manner.
- VPC Provisioning: The project provisions a VPC infrastructure with public and private subnets spread across multiple availability zones.
- High Availability: The infrastructure is designed to be highly available by distributing resources across different availability zones.
- Automated Deployment: GitHub Actions is used to automate the deployment process, making it easier to maintain and manage the infrastructure.

## Requirements

- AWS Account: Access to an AWS account to provision the infrastructure resources.
- AWS Credentials: Valid AWS access key ID and secret access key with appropriate permissions.
- Terraform: Installed Terraform CLI version 0.13.0 or higher on your local machine.
- GitHub Repository: A GitHub repository to store the project code and utilize GitHub Actions.

Ensure that the AWS credentials are securely stored and properly configured in the environment or as GitHub secrets.
 
AWS Credentials: Setup your AWS credentials. This can be done using the AWS CLI:

    aws configure   
    
## Usage

Clone the Repository

  bash
  
    git clone <your-repo-link>
    cd <your-repo-directory>

Initialize Terraform

bash

    terraform init

Apply the Changes

    terraform apply

Enter yes when prompted.

Destroy Resources (If Needed)

    terraform destroy

Enter yes when prompted.

## Conclusion

Notes
Ensure you have the necessary permissions in AWS to create these resources.
The S3 bucket for Terraform state has forced destroy enabled. Backup any important data.
Make sure the S3 bucket name you provide follows AWS naming conventions.
If deploying in an automated environment, ensure AWS credentials are accessible in that environment.
Adjust the provider region in the configuration if deploying to a region other than us-east-1.
