# Deploy a high-availability web app using CloudFormation
This project shows how to deploy web servers for a highly available web app using CloudFormation. The scripts create the network from scratch and deploy the virtual machines used to expose the application code present in an S3 Bucket.

## Cloud Architecture Diagram
![alt text](https://github.com/fabio-jaremciuc/[cloud-devops-engineer-udacity/deploy-web-app-aws/image/blob/master/network-diagram.png?raw=true)

## How to launch the scripts
1. To deploy the network infrastructure it is necessary run the follow bash script from the project folder: `./create.sh network network.yml network.json`
2. After the first point is successfully performed, run the second script to deploy the servers: `./create.sh servers servers.yml servers.json`
3. To delete all stacks miplemented run first `./delete.sh network` and after the network is deleted launch `./delete.sh servers`
