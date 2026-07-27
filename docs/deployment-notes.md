# Deployment Notes

## Phase 1 - Azure Infrastructure

Date:
27 July 2026

## Completed

- Created Azure Resource Group: security-lab
- Deployed Windows Server 2025 VM
- Enabled Trusted Launch
- Enabled Secure Boot and vTPM
- Created Virtual Network and Subnet
- Configured Network Security Group
- Restricted RDP access to authorized IP address
- Enabled VM auto-shutdown for cost control

## Security Considerations

RDP access was restricted through Azure NSG rules instead of exposing port 3389 to the entire internet.

## Next Steps

- Install Sysmon
- Configure Azure Monitor Agent
- Connect Microsoft Sentinel
- Create KQL detection rules
