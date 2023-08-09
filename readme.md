# BEFORE USING
## Add these variables to your gitlab(or bitbucket/github)'s variables
[Gitlab's variable config](https://gitlab.com/groups/demo4515608/-/settings/ci_cd)
> - SSH_SERVER_IP: your vps's ip
> - SSH_PRIVATE_KEY: private key (generated by ssh key-gen) of the device that has access to your vps

## Modify these variables
> - DOCKER_IMAGE_NAME: image name
> - DOCKER_IMAGE_TAG: image tag
> - PORT: port to expose after deploy
> - ENV_PATH: part of your .env file on server
Example:
> - DOCKER_IMAGE_NAME: "demo-auth-service"
> - DOCKER_IMAGE_TAG: "latest"
> - PORT: "3001"
> - ENV_PATH: "/home/minh/var/www/${DOCKER_IMAGE_NAME}/.env"