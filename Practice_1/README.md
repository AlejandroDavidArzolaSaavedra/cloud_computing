# AWS Cloud Computing - Practice 1 README

## 📋 Table of Contents
- [📖 Introduction](#introduction)
- [🚀 Prerequisite](#prerequisite)
- [🌟 Practice Overview](#practice-overview)
- [🚀 Part 1: Launching EC2 Instance](#part-1-launching-ec2-instance)
- [🚧 Part 2: Extending the Setup](#part-2-extending-the-setup)
- [🚢 Part 3: Deploying Moodle](#part-3-deploying-moodle)

## 📖 Introduction
This README provides a step-by-step guide for the first practice in Cloud Computing using AWS. In this practice, we will cover three parts to help you get started with AWS services and configurations.

## 🚀 Prerequisite
Before you begin, make sure you have the following:
- An AWS account (you can sign up at [AWS](https://aws.amazon.com/))
- AWS CLI installed and configured with your AWS credentials

## 🌟 Practice Overview
The first practice is divided into three parts:

### 🚀 Part 1: Launching EC2 Instance

In this part, we will launch an EC2 instance and open two ports: 80 for HTTP and 22 for SSH. We will then verify that we can access the instance and that the HTTP page is accessible.

Step-by-Step Instructions:
- Security Group Creation
- Open the AWS CloudFormation console.
- Upload the provided JSON template.
- Create a new stack, name it appropriately.
- EC2 Instance Launch
- Navigate to the EC2 dashboard.
- Identify the launched instance.
- Verify the open ports: 80 (HTTP) and 22 (SSH).
- Connect to the instance using SSH.
- Ensure the HTTP page is accessible via the public IP.

### 🚧 Part 2: Extending the Setup
Building upon the setup from Part 1, we will create two instances. The first instance (SSHGateInstance) will have SSH access from external sources (port 22), and the second instance (WebServerInstance) will only allow SSH access from the first instance. Additionally, the second instance will also host the HTTP service, requiring ports 80 and 22 to be open.

Step-by-Step Instructions:
- Security Group for SSH Gate (SSHGateSecurityGroup)
- This security group allows SSH access from any source (0.0.0.0/0).
- It will be associated with the SSHGateInstance.
- Security Group for Web Server (WebServerSecurityGroup)
- This security group allows SSH access only from the SSHGateSecurityGroup on port 22.
- It also allows HTTP access from any source on port 80.
- It will be associated with the WebServerInstance.
- Launching SSH Gate Instance (SSHGateInstance)
- This EC2 instance is configured to have SSH access from any source.
- It installs and starts the SSH service.
- Launching Web Server Instance (WebServerInstance)
- This EC2 instance is configured with security groups:
- WebServerSecurityGroup for SSH and HTTP access.
- It installs and starts the HTTP service and sets up a simple webpage.
- Verification
- Connect to the SSHGateInstance using SSH.
- Attempt to SSH into the WebServerInstance from the SSHGateInstance.
- Access the webpage hosted by the WebServerInstance via its public IP.

### 🚢 Part 3: Deploying Moodle
Continuing from Part 2, we will make Moodle available within the setup. 

## 🌝 Wrapping Up

Feel free to reach out if you have any questions or need further assistance.

Happy learning and cloud computing! 🌟🚀
