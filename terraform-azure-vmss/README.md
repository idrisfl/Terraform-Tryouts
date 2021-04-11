https://docs.microsoft.com/en-us/azure/developer/terraform/create-vm-scaleset-network-disks-hcl%20

terraform init

(multiple times)

terraform plan -out azure-vmss.plan
terraform apply "azure-vmss.plan"


terraform plan -destroy -out azure-vmss.destroy.tfplan
terraform apply "azure-vmss.destroy.tfplan"
