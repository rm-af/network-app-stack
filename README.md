# AWS CloudFormation Stack

This repository provides **AWS CloudFormation** templates for building a simple infrastructure:

- **network.yaml** → Creates the core network (VPC, subnets, internet gateway, and route tables).
- **app.yaml** → Launches an EC2 instance inside the created network.

## How to Use
1. Clone this repo:
   ```bash
   git clone https://github.com/rm-af/network-app-stack.git
   cd network-app-stack

2. Deploy Network:
  ```bash
  aws cloudformation create-stack --stack-name my-network --template-body file://network.yaml
```

3. Deploy App:
   ```bash
     aws cloudformation create-stack --stack-name my-app --template-body file://app.yaml

4.Requirements
AWS CLI installed and configured
IAM permissions for VPC & EC2
Active AWS account

