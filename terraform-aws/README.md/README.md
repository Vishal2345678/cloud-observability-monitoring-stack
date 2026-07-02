terraform-aws
Terraform AWS EC2 provisioning

Hit the Star! ⭐
If you are planning to use this Terraform repo for learning, please hit the star. Thanks!

EC2 Instance Provisioning
Navigate to the environment/dev/ec2 folder:
cd prometheus-stack/
Open the ec2.tfvars file and modify it with your desired details. This file contains variables used in the Terraform configuration.
Deployment
Format Terraform code per HCL canonical standards in the working directory:
terraform fmt
Validate Terraform code in the working directory:
terraform validate
Initialize Terraform in the working directory:
terraform init
Create an execution plan:
terraform plan --var-file=../vars/ec2.tfvars
Apply the changes to create the EC2 instance:
terraform apply --var-file=../vars/ec2.tfvars
To destroy the EC2 instance and associated resources:
terraform destroy --var-file=../vars/ec2.tfvars
Note: Always review the execution plan (terraform plan) before applying changes to avoid unintended modifications.

Terraform Command Reference
Update all outputs:

terraform refresh
Show all outputs:

terraform show