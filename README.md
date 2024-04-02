Terraform Project Documentation: Launching VPC with Subnets, EC2 Instances, and Load Balancer

1. Introduction

    This document serves as documentation for the Terraform project aimed at launching a Virtual Private Cloud (VPC) with two subnets, EC2 instances within the subnets, and an Application Load Balancer (ALB) to distribute traffic. The project also includes modularization for scalability and maintainability and integration with GitHub Actions for Continuous Integration/Continuous Deployment (CI/CD).

2. Project Overview

    The project aims to automate the provisioning of AWS infrastructure using Terraform, facilitating the deployment of a scalable and reliable architecture for hosting applications. The key components of the 
    project include:

    Creation of VPC with appropriate CIDR block
    Creation of two subnets within the VPC: public and private
    Launching EC2 instances within the subnets
    Configuring an Application Load Balancer (ALB) to distribute incoming traffic to the EC2 instances
    Modularization of Terraform code for better organization and reuse

3. Architecture Diagram


4. Terraform Modules

   The project is organized into several Terraform modules to encapsulate logical components and enable reuse across different environments. The modules include:

    vpc: Responsible for creating the VPC and its associated components.
    subnets: Creates the public and private subnets within the VPC.
    ec2: Launches EC2 instances within the subnets.
    alb: Configures the Application Load Balancer to distribute traffic to the EC2 instances.
 
5. GitHub Actions for CI/CD

    The project utilizes GitHub Actions for automating the CI/CD pipeline. Key features of the CI/CD pipeline include:

    Continuous Integration: Running Terraform validation and formatting checks on every pull request.
    Continuous Deployment: Automatically applying Terraform changes to the infrastructure upon merging changes into the main branch.

6. Conclusion

    The Terraform project provides a streamlined approach to provisioning AWS infrastructure for hosting applications. By leveraging modularization and CI/CD practices, the project ensures scalability, 
    reliability, and maintainability of the infrastructure.
