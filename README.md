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
├── main.tf          # S3 bucket & lifecycle configuration
├── provider.tf      # AWS provider configuration
├── variables.tf     # Input variable definitions
├── terraform.tfvars # Variable values
├── outputs.tf       # Output values

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
