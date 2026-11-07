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
## Lab Screenshots

### 1. Azure Virtual Machine Setup

Created and deployed the Windows Server 2022 virtual machine in Microsoft Azure.

![Creating a VM](./Creating%20a%20VM.png)

![VM Created](./VM%20created.png)

### 2. Active Directory Installation and Configuration

Installed the required server roles and promoted Windows Server 2022 to a Domain Controller.

![Selecting Server Roles](./Clicking%20What%20roles%20to%20install.png)

![Promoting Server to Domain Controller](./Promoting%20the%20server%20to%20a%20domain.png)

### 3. Network and DNS Configuration

Configured the Domain Controller's network settings and DNS so other machines could locate and communicate with the domain.

![Static IP Configuration](./setting%20up%20static%20IP_for%20domain%20Controller.png)

![DNS Configuration](./Setting%20up%20my%20DNS%20to%20connect%20to%20my%20domain%20controller.png)

![Verifying DNS Settings](./making%20sure%20it%20connects%20to%20the%20correct%20DNS%20IP.png)

![Testing Network Connectivity](./cmd_PING_and%20should%20work.png)

### 4. Active Directory User and Group Management

Created an Organizational Unit, configured domain user accounts, and created security groups.

![Creating an Organizational Unit](./Then%20open%20AD%20and%20create%20an%20organztional%20unit.png)

![Creating a Domain User](./creating%20a%20user.png)

![Creating a Security Group](./creating%20a%20group.png)

### 5. Group Policy Management

Worked with Group Policy Management and created Group Policy Objects (GPOs).

![Creating Group Policy Objects](./creating%20GPOs.png)

### 6. Joining a Second Server to the Domain

Created a second Windows Server 2022 virtual machine, configured it to communicate with the Domain Controller, and connected it to the Active Directory domain.

![Setting Up Second Virtual Machine](./setting%20up%20another%20VM%20to%20connect%20to%20domain%20controller.png)

![Connected to Domain Controller](./now%20connected%20to%20the%20domain%20controller.png)
