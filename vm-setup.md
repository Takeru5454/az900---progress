First Virtual Machine Setup


Task: Create resource group then a Linux VM
***************
az group create --name IntroAzureRG --location eastus

az vm create \
--resource-group "IntroAzureRG" \
--name my-vm \
--size Standard_D2s_v6 \
--public-ip-sku Standard \
--image Ubuntu2204 \
--admin-username azureuser \
--ssh-key-values "$(cat ~/.ssh/id_rsa.pub)"
***************

# Standard_D2s_v5 was not available in my region so I used az vm list-sizes --location eastus --output table Standard_D2s_v6 was available
# Instead of --generate-ssh-keys I used --ssh-key-values "$(cat ~/.ssh/id_rsa.pub)" --generate-ssh-keys was causing errors and couldnt generate my VM
# Using --ssh-key-values manually generates public keys and avoids the [Errno 5] Input/Output error

Task: Install Nginx
***************
az vm extension set \
--resource-group "IntroAzureRG" \
--vm-name my-vm \
--name customScript \
--publisher Microsoft.Azure.Extensions \
--version 2.1 \
--settings '{"fileUris":["https://raw.githubusercontent.com/MicrosoftDocs/mslearn-welcome-to-azure/master/configure-nginx.sh"]}' \
--protected-settings '{"commandToExecute": "./configure-nginx.sh"}'
***************

# Apparently it "Runs apt-get update to download the latest package information from the internet. Installs Nginx. Sets the home page, /var/www/html/index.html, to print a welcome message that includes your VM's host name."
