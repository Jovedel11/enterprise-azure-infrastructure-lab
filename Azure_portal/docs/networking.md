# Enterprise Azure Infrastructure Lab - Networking Phase

## Objective

Design and deploy a segmented Azure virtual network and create a NSG then associate it to designated subnets.

## Network Architecture

| Component | CIDR |
| VNet | 10.0.0.0/16 | - My actual network/Private cloud Network
| default | 10.0.0.0/24 | - My default network, it's like to contain some compute (VMs, Containers, ect.)
| Frontend Subnet | 10.0.1.0/24 | - Public Facing resources
| Backend Subnet | 10.0.2.0/24 | - Internal Systems
| Management Subnet | 10.0.3.0/16 | - Administrative access/Bastion

## Design Decisions

- Separate frontend and backend workloads/resource group
- Isolate management traffic
- Seperate subnet for Bastion deployment
- No Public IP for Windows VM (Bastion Connection)
- Apply least privilege network design
- Associate NSG to each Subnets

## Expected Learnings

- Azure VNets
- Subnets
- CIDR planning
- Network segmentation
- NSG Implementation