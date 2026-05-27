## Project Overview

- This project focuses on building a simulated enterprise cloud infrastructure environment in Microsoft Azure using core cloud, networking, security, monitoring, and hosting services. The main objective of the project is to gain real-world hands-on experience in Azure administration, infrastructure deployment, cloud operations, and troubleshooting as preparation for Cloud Engineer, System Administrator, and Azure-related roles.

- The infrastructure was designed and configured manually through the Azure Portal to strengthen practical understanding of how enterprise cloud environments are managed in real-world scenarios.

## Project Goals

The project aims to:

- Understand Azure core infrastructure services through hands-on implementation
- Learn virtual networking concepts such as VNets, subnets, NSGs, and public/private access
- Practice Linux VM administration and secure remote access using Azure Bastion
- Deploy and manage web services inside Azure infrastructure
- Explore Azure monitoring, logging, and operational visibility
- Learn cloud resource organization, troubleshooting, and cost management
- Simulate enterprise-style cloud architecture using Azure services

## Infrastructure Strategy

The project follows a simplified enterprise infrastructure design strategy where resources are separated logically for security, scalability, and manageability.

The strategy includes:

- Using Resource Groups for centralized infrastructure management
- Separating workloads using multiple subnets
- Applying Network Security Groups (NSGs) for traffic control and security
- Using Azure Bastion instead of exposing SSH publicly
- Hosting web services inside Linux virtual machines
- Integrating monitoring and logging services for operational visibility
- Using GitHub deployment workflows for cloud-hosted applications

## The project prioritizes:

- Security
- Operational visibility
- Hands-on troubleshooting
- Cost-awareness using Azure for Students subscription

## Infrastructure Architecture

Internet
│
▼
Azure Resource Group
│
├── Virtual Network (10.0.0.0/16)
│ ├── Frontend Subnet (Separate RG)
│ ├── Backend Subnet (Separate RG)
│ └── AzureBastionSubnet
│
├── Network Security Groups (Separate RG)
│
├── Azure Bastion
│
├── Linux Virtual Machine
│ └── NGINX Web Server
│
├── Azure Monitor
│
├── Log Analytics Workspace
│
└── Azure App Service (Separate RG)
└── GitHub Deployment

## Key Learnings

Throughout the project, the following skills and concepts were developed:

## Cloud Infrastructure

- Resource Group management
- Azure service deployment
- Infrastructure organization

## Networking

- VNets and subnetting
- Public vs private access
- NSG rule configuration
- Routing and secure access concepts

## Compute & Administration

- Linux VM deployment
- SSH administration
- NGINX installation and management
- Web hosting inside Azure

## Security

- Azure Bastion implementation
- Controlled administrative access
- Network traffic restriction using NSGs

## Monitoring & Operations

- Azure Monitor integration
- Log Analytics usage
- Metrics and infrastructure visibility
- Troubleshooting deployment and runtime issues

## DevOps & Deployment

- GitHub repository integration
- App Service deployment workflows
- Runtime compatibility troubleshooting

## Project Outcome

- The project successfully demonstrates foundational cloud engineering and infrastructure administration skills using Microsoft Azure. It provides practical exposure to networking, compute, security, monitoring, and cloud operations while simulating a real enterprise-style cloud environment.
