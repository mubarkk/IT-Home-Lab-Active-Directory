# Enterprise IT Home Lab: Active Directory & Windows Server 2022

## 🎯 Project Overview
This project involved architecting a virtualized enterprise network to simulate a real-world corporate environment. The goal was to practice core System Administration and Service Desk tasks, specifically focusing on user identity management, network services, and security permissions.

## 🛠️ Technical Stack
* **Hypervisor:** Oracle VirtualBox
* **Server OS:** Windows Server 2022 (Domain Controller)
* **Client OS:** Windows 11 Enterprise
* **Services:** Active Directory Domain Services (AD DS), DNS, DHCP

## 🚀 Key Implementation Steps

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

## 🛠️ Service Desk Scenarios Simulated
To prepare for high-volume support roles, I performed the following "Tickets":
* **Account Lockouts:** Diagnosed and resolved user login failures using AD Administrative Center.
* **Password Resets:** Managed secure password resets and forced "change at next logon" requirements.
* **Permission Requests:** Adjusted Security Group memberships to grant/revoke access to shared folders.
