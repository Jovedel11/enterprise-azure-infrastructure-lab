# Enterprise Azure Infrastructure Lab - Networking Phase

## Objective

Create and deploy VM with Linux Server with having a best size and storage fot it. And apply the Networking i create to it and setup SSH and NGINX installation.

## Network Architecture

VM specs:
- Size (B-Series V2)
- Storage (Standard SSD (LRS))

## Design Decisions

- For size, B-Series was perfect because, for only using AZ Student I priritize the cost so that's why I run it with AZ Spot Discount also, this was good because I only creating this for my LAB/Personal Project.
- No redundancy required and Standard Security type only
- For Storage Standard SSD was fine and using a disk size by default because this is for LAB only.
- The Virtual Network was Automatically attach because of being in Same region
- After Deploy the VM, i connect it using SSh and install a NGINX

## Expected Learnings

- Deploy VM with appropriate size and strorage
- Cost Management
- Network implementation
- NSG Implementation
- SSH, NGINX