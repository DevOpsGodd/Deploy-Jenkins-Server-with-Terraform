# Deploy-Jenkins-Server-with-Terraform

### This repository contains Terraform configuration files for deploying a Jenkins server on AWS EC2 instance as well as a script to install Terraform, git and kubectl on the instance.

#### Prerequisites
Before you can deploy the Jenkins server, you'll need to have the following prerequisites:

An AWS account with IAM user credentials that have permissions to create EC2 instances and security groups.
Terraform installed on your local machine.

#### How to use this repository
To deploy the Jenkins server, follow these steps:

- Clone this repository to your local machine. CD into the folder.

- In your AWS console, create a new keypair.  then Jenkins-server.tf file, update your keypair in the file.

Run the following commands from the root of the cloned repository:

```
terraform init
terraform plan
terraform apply
```
Terraform will prompt you to confirm that you want to create the resources. Enter yes to proceed.

Wait for Terraform to create the server. This can take a few minutes.

Once Terraform has finished creating the resources, you can SSH into the Jenkins server using the public IP address of the EC2 instance.

In a web browser, navigate to the public IP address of the EC2 instance to access the Jenkins web interface.
