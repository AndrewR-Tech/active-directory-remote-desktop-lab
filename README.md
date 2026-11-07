
# Windows Server 2022 - Active Directory Home Lab

## Overview
Hands-on lab configuring a Windows Server 2022 Active Directory environment, managing domain users and groups, implementing Group Policy, and configuring Remote Desktop access.

## Lab Environment
- Windows Server 2022 Domain Controller
- Windows Server 2022 Destination Server
- Active Directory Domain Services (AD DS)
- Group Policy Management
- Azure Bastion
- PowerShell


## Projects & Tasks

### 1. Active Directory User Management
- Created and managed domain user accounts.
- Worked with Active Directory Users and Computers.
- Configured user account properties and permissions.

### 2. Group Policy Management
- Worked with Group Policy to manage domain settings.
- Explored Group Policy Objects (GPOs).
- Practiced configuring and applying policies within the domain.

### 3. Remote Desktop Configuration
- Enabled Remote Desktop on a domain-joined Windows Server.
- Added domain users to the local Remote Desktop Users group.
- Configured remote login permissions.
- Tested remote authentication using domain credentials.

### 4. PowerShell Administration

Commands used to manage remote access:

```powershell
Add-LocalGroupMember -Group "Remote Desktop Users" -Member "LAB\ramzi.doe"

Get-LocalGroupMember -Group "Remote Desktop Users"
```

## Key Concepts & Skills
- Active Directory Domain Services
- User and Group Management
- Group Policy Objects (GPOs)
- Remote Desktop Services
- Windows Server 2022 Administration
- PowerShell
- Domain Authentication
- Access Control and Permissions
- Virtual Machine Management

## Outcome
Built hands-on experience managing a Windows Server 2022 Active Directory environment, configuring Group Policy, managing domain accounts, and troubleshooting Remote Desktop access between domain joined servers.
