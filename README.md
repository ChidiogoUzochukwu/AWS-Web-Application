# AWS-Web-Application

SmartShop Web Infrastructure Project


Overview


This project involves building a scalable and secure web application infrastructure for SmartShop, a fictional mid-sized retail company expanding into e-commerce. The solution leverages Amazon Web Services (AWS) to create a robust platform that ensures high availability, strong security, and cost-effectiveness.

With a limited budget and minimal in-house IT expertise, SmartShop requires a cloud-based infrastructure that is simple to manage and capable of growing with the business.


Objectives


The primary objectives of this project are:

Support Anticipated Growth:
Design an infrastructure that allows flexible resource allocation to handle traffic spikes during marketing campaigns and seasonal sales.

Ensure High Availability:
Leverage AWS services to provide redundancy and consistent uptime across multiple Availability Zones.

Strengthen Security:
Implement best practices for securing customer data and the overall infrastructure.

Optimize Costs:
Build a cost-effective solution that avoids over-provisioning while maintaining performance.


Key Components
1. Amazon EC2
Purpose: Hosts the web application.
Configuration: Instance was launched in the Ireland region using the Amazon Linux 2 AMI. Apache web server was installed to serve the application.
2. Virtual Private Cloud (VPC)
Purpose: Isolates the network environment.
Configuration: I made use of already created VPC that was divided into public and private subnets across multiple Availability Zones to ensure redundancy. I selected the public t2
3. Security Groups
Purpose: Provides instance-level traffic control.
Configuration:
I created a Security Group that allowed SSH and HTTP traffic from the internet.
   
Security Best Practices
1. Network Security: Network Access Control Lists (NACLs) were implemented for additional subnet-level protection.
2. IAM Roles: Assigned to instance to securely manage AWS resource access.


Cost Optimization


To maintain cost-efficiency, the project employed:
t2. micro Instance: Chosen for its low cost and suitability for the current scale





STEP BY STEP GUIDE OF WHAT I DID


Using an already created VPC and Public Subnet, I created a security group named: ChidiogoGinikaUzochukwu_litaSG allowing SSH and HTTP as the inbound rule.

I went ahead to Launch my Instance named : ChidiogoGinikaUzochukwu_lita, i selected Amazon Linux 2 as the OS and a t2.micro instance type.te

I selected the already created VPC and Subnet. I created a key pair named: ChidiogoGinikaUzochukwu_litaKP which was downloaded to my laptop.
The Auto-assign Public IP was also Enabled. I crosschecked the information and launched my Instance.


I went to the download folder of my laptop, located the key pair, right clicked and selected Git Bash Here
I entered the right commands, which also included commands to install Apache

I confirmed Apache is running by visiting the instance’s public IP address in a browser.


All screenshots are attached






Public IP Address of EC2 Instance: 54.72.96.88
