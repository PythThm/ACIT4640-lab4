# ACIT4640 Lab 4 Instructions
# Command for key gen
`ssh-keygen -t ed25519 -C "my-cloud-init-key" -f ~/.ssh/my_ssh_key` 
# For getting public key
`cat ~/.ssh/my_ssh_key.pub`
# To login with aws, use environmental variable
```
export AWS_ACCESS_KEY_ID="your-access-key-id"
export AWS_SECRET_ACCESS_KEY="your-secret-access-key"
export AWS_REGION="your-region"  # Example: us-east-1
```
# Commands for Terraform
```
terraform init        # Initialize Terraform
terraform validate    # Validate the .tf file
terraform plan        # View the changes
terraform apply       # Deploy setup from .tf file
terraform output      # View outputs
terraform destroy     # Remove everything
```

# Resources used
https://spacelift.io/blog/terraform-ec2-instance \
https://learning-ocean.com/tutorials/terraform/terraform-user-data/ \
https://cloudinit.readthedocs.io/en/latest/howto/index.html \
https://registry.terraform.io/providers/hashicorp/aws/latest/docs
