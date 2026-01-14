# "Hello, World!" Website on AWS

## Overview
Deploy a simple "Hello, World!" website using AWS and Terraform. The project includes a scalable, globally distributed architecture with S3, CloudFront, and EC2.

## Features
- Static website hosting on S3
- Global distribution with CloudFront
- Auto Scaling for EC2 instances
- Infrastructure as Code using Terraform

## Technologies
- AWS (S3, CloudFront, EC2, Auto Scaling)
- Terraform
- HTML

## Setup / Installation
1. Clone the repository:
```bash
git clone https://github.com/sabihadudhia/hello-world-website.git
cd hello-world-website
```
2. Update configuration:
- Open provider.tf and set AWS region if needed
- Replace subnet IDs or other specific resource IDs with your own
- Initialize and deploy with Terraform:
```bash
terraform init
terraform plan
terraform apply
```

## Usage
- Access the website via the CloudFront URL or S3 endpoint provided in Terraform outputs
- Modify index.html in the S3 bucket to change website content

## Project Structure
```bash
├── provider.tf        # AWS provider configuration
├── S3.tf              # S3 bucket setup
├── CloudFront.tf      # CloudFront distribution setup
├── EC2.tf             # EC2 and Auto Scaling configuration
├── index.html         # Static HTML file
└── README.md          # Documentation
```

## Outputs
- S3 Website Endpoint: direct access to static website
- CloudFront Distribution URL: globally cached website address
