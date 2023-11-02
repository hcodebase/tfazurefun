# Prerequisites
- An Azure account with active subscription
- Terraform installed on your local machine
- Azure CLI installed and configured

If you haven't done so, follow the [instruction here](https://developer.hashicorp.com/terraform/tutorials/azure-get-started/azure-build#authenticate-using-the-azure-cli) to set up your Terraform authenticate using Azure CLI

# Set Variables
Chagne the project and location settings to use your own value
```
project  = "tfexample"
location = "australiaeast"
```

# Add Your Azure Function Code (Optional)
```
git submodule add {Your function git repository}
```

# Deploy
```
terraform init
terraform apply -auto-approve
```