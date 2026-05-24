# Enterprise Azure Infrastructure Lab - Security Phase

## Objective

NSG is Network Security Group, it acts a firewall for each subnet. So, my goal is to apply allow and deny security for each subnet. So having a public ip for Linux VM, The Windows Server VM was deployed without a public IP address.

## Security Architecture

Linux Server (Public Side)
- Enbale Public IP
- Allow SSH
- Install NGINX
- Implement to nsg-frontend(public figure)

Windows Server (Private Side)
- Deny Public
- Not allow any port
- Access using Bastion
- Implement t0 nsg-backend(private figure)

## Design Decisions

- Allow SSH for my frontend NSG so it will be the preperation for my Linux VM Later.
- For now i just donnot allow public inbound traffic for my backend.
- Administrative access is performed securely through Azure Bastion,
which eliminates the need to expose RDP (3389) directly to the internet.

## Expected Learnings

- Simple Firewalling
- Access Control
- Least Priviledge
- Bastion Approach and not using RDP approach follows security best practices and reduces attack surface exposure.