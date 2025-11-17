First Virtual Machine Setup

***************
- az group create --name IntroAzureRG --location eastus

- az vm create --resource-group "IntroAzureRG" \
--name my-vm \
--size Standard_D2s_v6 \
--public-ip-sku Standard \
--image Ubuntu2204 \
--admin-username azureuser \
--generate-ssh-keys

# Standard_D2s_v5 was not available in my region so 
