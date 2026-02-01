## 📦 Terraform AWS S3 Bucket with Lifecycle Policy
🧾 Project Description

This project uses Terraform to provision an AWS S3 bucket and apply a lifecycle policy to manage storage efficiently by transitioning and expiring objects automatically.

🛠️ What This Project Does

-Creates an S3 bucket with custom tags

-Applies a lifecycle rule:

-Moves objects to STANDARD_IA after 30 days

-Deletes objects after 365 days

-Uses variables and tfvars for flexible configuration

-Outputs the bucket name and ARN

🧩 Terraform Files Structure
.
main.tf          # S3 bucket & lifecycle configuration
   |
provider.tf      # AWS provider configuration
   |
variables.tf     # Input variable definitions
   |
terraform.tfvars # Variable values
   |
outputs.tf       # Output values


🚀 How to Run This Terraform Project

Follow these steps to provision the AWS S3 bucket using Terraform:

1️⃣ Initialize Terraform

Initializes the working directory and downloads the required provider plugins.

terraform init

2️⃣ Review the Execution Plan

Shows what resources Terraform will create before applying changes.

terraform plan

3️⃣ Apply the Configuration

Creates the S3 bucket and attaches the lifecycle policy.

terraform apply


Type yes when prompted.

4️⃣ (Optional) Destroy the Resources

Removes all resources created by Terraform.

terraform destroy

⚠️ Prerequisites

AWS account

AWS CLI configured (aws configure)

Terraform installed

IAM user with S3 permissions

🧠 Why init, plan, apply Matter

terraform init → prepares Terraform to work

terraform plan → prevents accidental changes

terraform apply → safely provisions infrastructure

🧠 Skills Demonstrated

Terraform Infrastructure as Code (IaC)

AWS S3

Lifecycle Management

Variables & Outputs

Environment-based configuration

📌 Use Case

This setup is useful for:

Cost-optimized storage management

Log archiving

Backup data lifecycle automation
