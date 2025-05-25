azure-rg-infra/
├── modules/
│   └── resource-group/
├── environments/
│   ├── dev/
│   ├── staging/
│   └── prod/
├── scripts/
├── main.tf
├── variables.tf
├── README.md
└── ...

🚀 Getting Started
Prerequisites
Terraform v1.0 or higher

Azure CLI

Access to an Azure subscription

Setup
Login to Azure:

bash
Copy
Edit
az login
Initialize the project:

bash
Copy
Edit
terraform init
Plan and apply:

bash
Copy
Edit
# Example for the dev environment
terraform plan -var-file="environments/dev/terraform.tfvars"
terraform apply -var-file="environments/dev/terraform.tfvars"
🔐 Security & Secrets
Secrets are not stored in the repository.

Use Azure Key Vault for managing sensitive data.

.tfvars and .env files are included in .gitignore.

📄 Contributing
We welcome contributions! Please fork the repo and submit a pull request.
Refer to the CONTRIBUTING.md for guidelines.

📜 License
Distributed under the MIT License. See LICENSE for more information.

🙋 FAQ
Q: What is a Resource Group in Azure?
A: A Resource Group is a container that holds related resources for an Azure solution. It allows you to manage and organize assets like VMs, databases, and networks collectively.

Q: Can this be used for multiple environments?
A: Yes! The repo supports environment-based configurations under the environments/ folder.

