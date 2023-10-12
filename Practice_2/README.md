# AWS Cloud Computing - Practice 2

## 📋 Table of Contents
- [📖 Introduction](#introduction)
- [🚀 Prerequisite](#prerequisite)
- [🌟 Practice Overview](#practice-overview)
- [🚀 Part 1: Deploying Web Servers](#part-1-deploying-web-servers)
- [🚧 Part 2: Load Balancing](#part-2-load-balancing)
- [🚢 Part 3: Auto Scaling and Load Balancing](#part-3-auto-scaling-and-load-balancing)
- [🌐 Part 4: Database Deployment (Optional)](#part-4-database-deployment-optional)
- [🌝 Wrapping Up](#wrapping-up)

## 📖 Introduction
This README provides a step-by-step guide for the second practice in Cloud Computing using AWS. The focus of this practice is on database deployment, load balancing, and auto-scaling.

## 🚀 Prerequisite
Before you begin, make sure you have the following:
- An AWS account (you can sign up at [AWS](https://aws.amazon.com/))
- AWS CLI installed and configured with your AWS credentials

## 🌟 Practice Overview
The second practice is divided into four parts:

### 🚀 Part 1: Deploying Web Servers
In this part, we will deploy two EC2 instances with distinct web servers that can be accessed from a web browser.

Step-by-Step Instructions:
- Launch two EC2 instances with web servers.
- Configure each server to display a distinguishable webpage.
- Verify accessibility from a web browser.

### 🚧 Part 2: Load Balancing
Building upon the web server setup, we will deploy a load balancer to evenly distribute incoming requests between the two servers.

Step-by-Step Instructions:
- Set up an Elastic Load Balancer (ELB).
- Add the two web servers to the load balancer.
- Verify load balancing functionality.

### 🚢 Part 3: Auto Scaling and Load Balancing
Extend the setup by creating a template for EC2 instances, declaring an Auto Scaling Group (ASG) with a minimum of one instance and a maximum of two. The ASG should be added to the previously deployed load balancer.

Step-by-Step Instructions:
- Create an EC2 instance template.
- Declare an Auto Scaling Group with the template.
- Add the ASG to the existing load balancer.
- Verify that the ASG maintains at least one instance and receives incoming requests from the load balancer.

### 🌐 Part 4: Database Deployment (Optional)
For an optional activity, investigate and deploy a database of your choice within AWS. Demonstrate its functionality and estimate the cost of usage.

## 🌝 Wrapping Up
Feel free to reach out if you have any questions or need further assistance. Happy learning and exploring the capabilities of AWS! 🌟🚀
