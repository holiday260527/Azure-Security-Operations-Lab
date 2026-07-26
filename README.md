# cloud-security-lab
Personal Cloud Security Lab simulating a UK company.

Azure Security
Security Operations
Detection Engineering
Incident Response
Terraform
Automation






                     Internet
                         │
                  Azure Firewall
                         │
               security-lab-2026
                  10.0.0.0/16
                         │
        ┌────────────────┴────────────────┐
        │                                 │
 Management Subnet                 Production Subnet
    10.0.1.0/24                      10.0.2.0/24
        │                                 │
 nsg-management                     nsg-production
        │                                 │
 Azure Bastion                 ┌──────────┴──────────┐
                               │                     │
                          vm-win01             vm-linux01
