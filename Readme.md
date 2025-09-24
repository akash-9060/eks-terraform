# eks-terraform
A sample repository to create EKS on AWS using Terraform.
The purpose of this repo is to give you a very minimal EKS cluster for the purpose of learning Kubernetes using Terraform. The cluster is a great foundation for starting to learn what it might take to manage a production-ready Kubernetes cluster in AWS on EKS, deployed through Terraform. The starter is intentionally a minimal starter, and is not an entirely production-ready cluster (e.g. no remote state for terraform setup, the single node setup is insufficient, etc). The starter, however is a great jumping off point to start to iterate on the given configuration to add your own complexity and features yourself.




Prerequisite knowledge
=
You do not need to be a master of all of the below technologies, but you do at least need to know what they are, what they do, and be comfortable modifying them if you need to debug anything. For instance, if you have never deployed an EC2 instance into AWS using Terraform (or a similar tool), that would be a better starting point than this repository.

Linux - Installing packages, configuring environment variables and configuration files, using commands, flags, etc.

AWS Compute & Networking Foundations - e.g. EC2, Subnets, VPC.

Kubernetes - Understanding of the reasons for using Kubernetes, and basic terminology.## Install AWS CLI 

As the first step, you need to install AWS CLI as we will use the AWS CLI (`aws configure`) command to connect Terraform with AWS in the next steps.

Follow the below link to Install AWS CLI.
```
https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
```

### Install Terraform

Next, Install Terraform using the below link.
```
https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli
```

### Connect Terraform with AWS

Its very easy to connect Terraform with AWS. Run `aws configure` command and provide the AWS Security credentials.

### Initialize Terraform

Clone the repository and Run `terraform init`. This will intialize the terraform environment for you and download the modules, providers and other configuration required.

### Optionally review the terraform configuration

Run `terraform plan` to see the configuration it creates when executed.

### Finally, Apply terraform configuation to create EKS cluster with VPC 

`terraform apply`


