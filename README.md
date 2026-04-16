# Active-Directory-Lab


## Overview

- This lab demonstrates hands-on experience with Windows Server administration, network configuration, Group Policy management, and PowerShell scripting.
- Designed and deployed a fully functional Active Directory environment using VirtualBox to simulate a real enterprise network.



## Environment

# (Component | Details)
- Hypervisor - Oracle VirtualBox 
- Domain Controller - Windows Server 2022 
- Client Machine - Windows 10 Pro 
- Domain Name - corp.local 
- Network - Internal Network (192.168.10.0/24) 

## What Was Built

- Deployed Windows Server 2022 and promoted it to a Domain Controller
- Configured DNS and DHCP server roles on the domain controller
- Created an Organizational Unit structure for IT, HR, and Finance departments
- Created user accounts and security groups for each department
- Linked Group Policy Objects to enforce security policies
- Joined a Windows 10 Pro client machine to the domain
- Automated bulk user creation using PowerShell

## Group Policy Objects

# (Policy | Settings)
- Screen lock timeout - 600 seconds (10 minutes)
- Removable storage access - Disabled

## PowerShell Automation

- Used PowerShell to bulk create domain users across multiple Organizational Units
- Iterated through a predefined user array
- Created accounts with New-ADUser
- Assigned users to correct OUs automatically
- Verified creation with Get-ADUser

## Screenshots

# (See the /screenshots folder for documentation)
- Organizational Unit structure with users and security groups
- Group Policy Object configuration and settings
- PowerShell bulk user creation output
- CLIENT01 joined to corp.local domain

## Skills Demonstrated

- Windows Server 2022 administration
- Active Directory Domain Services (AD DS)
- DNS and DHCP configuration
- Group Policy management
- PowerShell scripting
- Network configuration and troubleshooting
- VirtualBox virtualization
