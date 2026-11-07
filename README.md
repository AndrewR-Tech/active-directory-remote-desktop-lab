# Windows Server 2022 - Active Directory Home Lab

## Overview
Built a hands-on Windows Server 2022 lab in Microsoft Azure to practice Active Directory administration, domain management, Group Policy, and Remote Desktop configuration.

## Lab Environment
- Microsoft Azure
- Azure Bastion
- Windows Server 2022 Domain Controller (Azure VM)
- Second Windows Server 2022 VM joined to the Active Directory domain
- Active Directory Domain Services (AD DS)
- Group Policy Management
- PowerShell

## Projects & Tasks

### 1. Active Directory Setup and User Management
- Installed and configured Active Directory Domain Services.
- Promoted a Windows Server 2022 VM to a Domain Controller.
- Created and managed domain user accounts.
- Worked with Active Directory Users and Computers.
- Configured user account properties and permissions.

### 2. Domain Join and Computer Configuration
- Created a second Windows Server 2022 virtual machine in Azure.
- Joined the second server to the Active Directory domain.
- Verified that the second server was communicating with the domain.
- Tested domain authentication using a domain user account.

### 3. Group Policy Management
- Worked with Group Policy Management.
- Explored and configured Group Policy Objects (GPOs).
- Practiced managing domain settings through Group Policy.

### 4. Remote Desktop Configuration
- Enabled Remote Desktop on the domain-joined server.
- Added a domain user to the local Remote Desktop Users group.
- Configured remote login permissions.
- Tested Remote Desktop access using domain credentials.
- Troubleshot and resolved a remote login permissions issue.

### 5. PowerShell Administration

Used PowerShell to manage local group membership and verify Remote Desktop permissions.

**Add a domain user to the Remote Desktop Users group:**

    Add-LocalGroupMember -Group "Remote Desktop Users" -Member "LAB\ramzi.doe"

**Verify group membership:**

    Get-LocalGroupMember -Group "Remote Desktop Users"

## Key Concepts & Skills
- Windows Server 2022 Administration
- Active Directory Domain Services (AD DS)
- Domain Controller Configuration
- Domain Joining
- User and Group Management
- Group Policy Objects (GPOs)
- Remote Desktop Configuration
- PowerShell
- Domain Authentication
- Access Control and Permissions
- Microsoft Azure Virtual Machines
- Azure Bastion

## Outcome
Built a two-server Windows Server 2022 environment in Azure, configured a Domain Controller, joined a second server to the domain, managed domain accounts, worked with Group Policy, and configured and tested Remote Desktop access using domain credentials.
