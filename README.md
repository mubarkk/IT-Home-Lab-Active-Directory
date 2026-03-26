# Enterprise IT Home Lab: Active Directory & Windows Server 2022

## Project Overview
This project involved architecting a virtualized enterprise network to simulate a real-world corporate environment. The goal was to practice core System Administration and Service Desk tasks, with a focus on user identity management, network services, and security permissions.

## Technical Stack
* **Hypervisor:** Oracle VirtualBox
* **Server OS:** Windows Server 2022 (Domain Controller)
* **Client OS:** Windows 11 Enterprise
* **Services:** Active Directory Domain Services (AD DS), DNS, DHCP

## Key Implementation Steps

### 1. Domain Controller Setup
- Installed and configured Windows Server 2022.
- Promoted the server to a Domain Controller for the forest `LAB.LOCAL`.
- Configured Static IP addressing and DNS forwarders to ensure reliable name resolution.

### 2. Active Directory Configuration
- **OU Structure:** Created Organizational Units (OUs) for Departments (HR, IT, Finance) and Security Groups.
- **User Management:** Scripted the creation of multiple test users with specific permission levels.
- **Group Policy:** Implemented GPOs for automated wallpaper branding and restricted Control Panel access for non-admin users.

### 3. Client Integration
- Provisioned a Windows 11 VM and successfully joined it to the `LAB.LOCAL` domain.
- Verified roaming profile functionality and mapped network drives via Login Scripts.

## Service Desk Scenarios Simulated
To prepare for high-volume support roles, I performed the following "Tickets":
* **Account Lockouts:** Diagnosed and resolved user login failures using AD Administrative Center.
* **Password Resets:** Managed secure password resets and forced "change at next logon" requirements.
* **Permission Requests:** Adjusted Security Group memberships to grant/revoke access to shared folders.

## Lab Evidence & Visual Documentation

### 1. Virtualized Infrastructure
![VirtualBox Manager](VirtualBox%20Manager.png)
*Figure 1: Oracle VirtualBox environment showing the Windows Server 2022 Domain Controller and Windows 11 Client, demonstrating virtualization management and resource allocation.*

### 2. Active Directory User & Group Management
![Active Directory Users & Computers](Active%20Directory%20Users%20%26%20Computers.png)
*Figure 2: ADUC interface displaying the custom Organizational Unit (OU) structure. This setup was used to practice the "User Access Management" skills required for Service Desk operations.*

### 3. Network Configuration Verification
![Command Prompt ipconfig](Command%20Prompt%20ipconfig.png)
*Figure 3: Successful 'ipconfig /all' results on the Windows 11 workstation, confirming proper DNS and DHCP communication with the Domain Controller.*

### 4. Help Desk Scenario: Account Troubleshooting
![Account Lockouts](Account%20Lockouts.png)
*Figure 4: Demonstration of account lockout resolution and password policy enforcement, simulating real-world high-volume support tickets.*

### 5. Successful Domain Authentication
![Windows 11 Lock Screen](Windows%2011%20Lock%20Screen.png)
*Figure 5: The Windows 11 client login screen showing a successful domain join. This confirms the workstation is fully integrated into the LAB.LOCAL forest and ready for user deployment.*

---
**[Return to Top](#enterprise-it-home-lab-active-directory--windows-server-2022)**
