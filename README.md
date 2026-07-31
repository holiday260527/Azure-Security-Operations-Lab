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

graph TD
    Internet --> AzureFirewall

    AzureFirewall --> VNet

    VNet --> AzureFirewallSubnet
    VNet --> ManagementSubnet
    VNet --> ProductionSubnet

    ProductionSubnet --> WindowsVM
    ProductionSubnet --> LinuxVM

    WindowsVM --> AMA
    AMA --> DCR
    DCR --> LogAnalytics
    LogAnalytics --> Sentinel
    ProductionSubnet --> LinuxVM
```

