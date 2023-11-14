# Using the Azure Developer CLI

Scratch space for notes and learning around Azure Developer CLI.

Create the template:

`azd init -t azure-search-openai-demo --debug`

Login to the tenant:

`azd auth login --use-device-code`

Create a resource group:

`az group create -n rg-genai-dev-001 -l uksouth --tags "productOwner=me@dat.com" "application=Generative AI" "environment=dev" "projectCode=n/a" --debug`

Examples of how to set environment variables in the Azure Developer CLI:

`azd config set defaults.location uksouth --debug`

`azd config set defaults.group rg-genai-dev-001 --debug`

Create and set the Python environments:

`conda create --name azd python=3.11`

`conda activate azd`

Install a node version:

`nvm install latest`

Create an environment file:

`node -r fs -e "fs.copyFileSync('sample-env', '.azure/dev/.env', fs.constants.COPYFILE_EXCL)"`

Deploy a specific environment using the Developer CLI:

`azd up -e dev`
