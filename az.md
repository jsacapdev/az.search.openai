# Using the Azure Developer CLI

Scratch space for notes and learning around Azure Developer CLI.

`azd init -t azure-search-openai-demo --debug`

`azd auth login --use-device-code`

`az group create -n rg-genai-dev-001 -l uksouth --tags "productOwner=me@dat.com" "application=Generative AI" "environment=dev" "projectCode=n/a" --debug`

`azd config set defaults.location uksouth --debug`

`azd config set defaults.group rg-genai-dev-001 --debug`

`conda create --name azd python=3.11`

`conda activate azd`

`nvm install latest`

`node -r fs -e "fs.copyFileSync('sample-env', '.azure/dev/.env', fs.constants.COPYFILE_EXCL)"`

`azd up -e dev`
