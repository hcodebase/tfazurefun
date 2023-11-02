# Prerequisites
- An Azure account with an active subscription
- Terraform installed on your local machine
- Azure CLI installed and configured

If you haven't done so, follow the [instructions here](https://developer.hashicorp.com/terraform/tutorials/azure-get-started/azure-build#authenticate-using-the-azure-cli) to set up your Terraform authenticate using Azure CLI

# Set Variables
Change the project and location settings to use your own value
```
project  = "tfexample"
location = "australiaeast"
```

# Add Your Azure Function Code (Optional)
```
git submodule add {Your function git repository}
```
# Update submodule (Optional)
If you will use the example code, update the submodule code before proceeding.
```
git submodule update --init --recursive
```

# Deploy
```
terraform init
terraform apply -auto-approve
```

# Clean up
Destroy the deployment:
```
terraform apply -destroy -auto-approve
```
