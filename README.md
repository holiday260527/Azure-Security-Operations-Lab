# cloud-security-lab
Personal Cloud Security Lab simulating a UK company.

## Focus Areas
- Azure Security
- Security Operations (SOC)
- Detection Engineering
- Incident Response
- Infrastructure as Code (Terraform)
- Automation

## Architecture Architecture  
```mermaid
graph TD
    Internet --> AzureFirewall[Azure Firewall]

    AzureFirewall --> VNet[Virtual Network]

    VNet --> ManagementSubnet[Management Subnet]
    VNet --> ProductionSubnet[Production Subnet]

    ProductionSubnet --> WindowsVM[Windows VM]
    ProductionSubnet --> LinuxVM[Linux VM]

    WindowsVM --> AMA[Azure Monitor Agent]
    AMA --> DCR[Data Collection Rule]
    DCR --> LAW[Log Analytics Workspace]
    LAW --> Sentinel[Microsoft Sentinel]
