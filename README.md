# cloud-security-lab
Personal Cloud Security Lab simulating a UK company.

## Objectives
This lab focuses on building practical cloud security skills:
Azure Security
Security Operations (SOC)
Detection Engineering
Incident Response
Infrastructure as Code (Terraform)
Automation

## Architecture Architecture  

```mermaid
graph TD
    Internet --> Firewall
    Firewall --> VNet
    VNet --> ManagementSubnet
    VNet --> ProductionSubnet
    ProductionSubnet --> WindowsVM --> AMA AMA --> DCR DCR --> LogAnalytics LogAnalytics --> Sentinel
    ProductionSubnet --> LinuxVM
```

