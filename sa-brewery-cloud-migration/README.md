# SA Brewery Cloud Migration (AWS Project)

## Overview
This project presents a cloud migration plan for SA Brewery, transitioning from an on-premises infrastructure to Amazon Web Services (AWS).

The goal is to improve scalability, security, cost efficiency, and operational flexibility using a rehost (lift-and-shift) strategy.

---

## Business Problem
SA Brewery operates on aging on-premises infrastructure with:
- Limited scalability
- High maintenance costs
- No cloud backup or redundancy
- Security risks due to outdated systems

As the company expands internationally, a modern and scalable cloud solution is required.

---

## Proposed Solution

A cloud-based architecture using AWS services:

- Amazon EC2 → hosts the web/CRM application  
- Amazon RDS (MySQL) → managed database service  
- Amazon VPC → secure network isolation  
- Public Subnet → web server (EC2)  
- Private Subnet → database (RDS)  
- Internet Gateway → external access  
- NAT Gateway → secure outbound access  

---

## Architecture Design

- Frontend (EC2) deployed in public subnet  
- Backend (RDS) deployed in private subnet  
- Security groups control communication  
- Database is not publicly accessible  

---

## Key Features

- Scalable infrastructure using AWS  
- Managed database with automated backups  
- Secure networking with VPC and subnets  
- Reduced operational overhead  
- Pay-as-you-go pricing model  

---

## Deployment Summary

1. Created a custom VPC  
2. Configured public and private subnets  
3. Attached Internet Gateway and configured routing  
4. Set up security groups (EC2 and RDS)  
5. Launched EC2 instance  
6. Deployed MySQL RDS instance  
7. Connected application to database  

---

## Cost Considerations

- Low-cost instances (t3.micro) used  
- No upfront hardware investment  
- Scalable pricing based on usage  

---

## Security Considerations

- Database isolated in private subnet  
- Security groups restrict access  
- Encryption and backups enabled  
- Secure SSH access using key pairs  

---

## Outcome

Successfully designed a scalable and secure cloud architecture that supports business growth, improves reliability, and reduces infrastructure complexity.

---

## Skills Demonstrated

- AWS Cloud Architecture Design  
- Amazon EC2 and RDS deployment  
- VPC, Subnets, and Networking  
- Security Groups and access control  
- Cloud cost and scalability planning

## Project Context

This project is based on an academic case study completed as part of the Cloud Platforms course at UniSA.

The task involved analysing an existing on-premises IT infrastructure and designing a cloud migration solution using AWS services. The solution was implemented as a prototype within the AWS Academy Learner Lab environment, following a rehost (lift-and-shift) strategy.

The full report included detailed technical analysis, cost considerations (CapEx vs OpEx), security planning, and deployment steps.
