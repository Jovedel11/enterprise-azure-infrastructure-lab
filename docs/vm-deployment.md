# Enterprise Azure Infrastructure Lab - Compute Phase (VMs)

## Objective

1. Create and deploy VM with Linux Server with having a best size and storage fot it. And apply the Networking i create to it and setup SSH and NGINX installation.

2. Create and deploy VM with Windows Server in backend side, which is not facing the public figures. So wihtout enabling the public ip, it have private and I will connect to Windwos VM by using Bastion.

## Compute Architecture

VM specs (Linux & Windows):
- Size (B-Series V2)
- Storage (Standard SSD (LRS))

Network (Linux):
- Attach to NSG frontend (Public Resources)
- Allow  SSH and HTTP(for NGINX)

Network (Windows):
- Attach to NSG backend (Backend/Private Side)
- No public ip, only Private
- Bastion enabled

## Design Decisions

- For size, B-Series was perfect because, for only using AZ Student I priritize the cost so that's why I run it with AZ Spot Discount also, this was good because I only creating this for my LAB/Personal Project.
- No redundancy required and Standard Security type only
- For Storage Standard SSD was fine and using a disk size by default because this is for LAB only.
- The Virtual Network was Automatically attach because of being in Same region
- After Deploy the VM, i connect to it using powershell and use SSH and install a NGINX (Linux)
- I allow for my nsg-frontend the http, so i can test in browse if my NGINX is active (Linux)
- After not allowing any public ip in my Windows Server, I enabled the Bastion for my connection for it (Linux)

## Expected Learnings

- Deploy VM with appropriate size and strorage
- Cost Management
- Network implementation
- NSG Implementation
- SSH, NGINX
- NSG security rules.