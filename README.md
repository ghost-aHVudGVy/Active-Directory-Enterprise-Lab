# Enterprise IT Lab Environment

This project demonstrates the design, deployment, and administration of a simulated enterprise IT environment using Windows Server 2022, Active Directory, Group Policy, Windows 10 Pro clients, and industry-standard IT management tools.  

The lab was built to replicate real-world corporate infrastructure, focusing on identity management, security policies, remote administration, software deployment, and help desk operations. It showcases practical skills expected of a Systems Administrator or IT Support Specialist.

---

## Objectives

- Build a fully functional Active Directory domain environment
- Configure domain-joined Windows 10 Pro clients
- Implement security policies with Group Policy Objects (GPOs)
- Manage users, computers, and organizational units (OUs)
- Configure file sharing, permissions, and drive mapping
- Demonstrate remote administration and troubleshooting methods
- Deploy and inventory software with PDQ tools
- Simulate real-world help desk operations with Spiceworks

---

## Environment Overview

- **Server Operating System:** Windows Server 2022 (Domain Controller)  
- **Client Operating System:** Windows 10 Pro (departmental machines for IT, HR, and Helpdesk)  
- **Tools and Utilities:** RSAT, PDQ Deploy, PDQ Inventory, Spiceworks, Account Lockout Tool  
- **Virtualization Platform:** VirtualBox (or VMware/Hyper-V)  

---

## Project Phases

### 1. Infrastructure Setup
- Installed Windows Server 2022 and configured base settings.  
![Server Manager](./screenshots/infrastructure/server-manager.png)

- Installed Windows 10 Pro virtual machines for IT and HR departments.  
![Windows 10 VM](./screenshots/infrastructure/win10-installation.png)

- Activated the Administrator account on clients and optimized performance.  
![Windows 10 Settings](./screenshots/infrastructure/win10-settings.png)

- Configured static IP addresses for server and clients.  
![IP Configuration](./screenshots/infrastructure/ipconfig.png)

- Verified connectivity using `ping`.  
![Ping Test](./screenshots/infrastructure/ping.png)

- Installed RSAT tools on Windows 10 for Active Directory management.  
![RSAT Installed](./screenshots/infrastructure/rsat.png)

---

### 2. Active Directory Domain Services
- Installed and configured Active Directory Domain Services (AD DS).  
![AD DS Installation](./screenshots/active-directory/adds-install.png)

- Promoted the server to a domain controller for the `corp.local` domain.  
![Domain Promotion](./screenshots/active-directory/domain-promotion.png)

- Enabled the Active Directory Recycle Bin for account recovery.  
![Recycle Bin Enabled](./screenshots/active-directory/recycle-bin.png)

- Created and managed Organizational Units (OUs) for IT, HR, and Helpdesk.  
![OU Structure](./screenshots/active-directory/ou-structure.png)

- Added users and computers to OUs.  
![User Accounts](./screenshots/active-directory/users.png)

- Delegated administrative control for specific departments.  
![Delegated Control](./screenshots/active-directory/delegate-control.png)

- Cloned and created user accounts to standardize provisioning.  
![Copy User](./screenshots/active-directory/copy-user.png)

---

### 3. Security and Group Policies
- Configured password complexity, history, and expiration.  
![Password Policy](./screenshots/policies/password-policy.png)

- Enabled and tuned account lockout policies.  
![Account Lockout](./screenshots/policies/account-lockout.png)

- Verified policy application using gpupdate and gpresult commands.  
![GPResult](./screenshots/policies/gpresult.png)

- Applied Group Policies to disable features such as Task Manager and Logoff.  
![Disabled Task Manager](./screenshots/policies/disable-taskmgr.png)

- Differentiated between security groups (access control) and distribution groups (communication).  
![Group Types](./screenshots/policies/groups.png)

---

### 4. File Sharing and Drive Management
- Created shared folders for HR and IT departments.  
![Shared Folder](./screenshots/drives/shared-folder.png)

- Configured NTFS and share-level permissions for security groups.  
![Folder Permissions](./screenshots/drives/permissions.png)

- Mapped drives manually and through Active Directory.  
![Mapped Drive](./screenshots/drives/mapped-drive.png)

- Verified access control for shared resources.  
![Access Verified](./screenshots/drives/access-test.png)

---

### 5. Remote Administration
- Accessed domain-joined machines through Remote Desktop.  
![RDP Session](./screenshots/remote-admin/rdp.png)

- Used Windows Remote Assistance for end-user support.  
![Remote Assistance](./screenshots/remote-admin/remote-assistance.png)

- Connected to administrative shares such as C$ for file management.  
![C$ Share](./screenshots/remote-admin/c-share.png)

- Accessed and modified the Windows Registry remotely.  
![Remote Registry](./screenshots/remote-admin/remote-registry.png)

---

### 6. Software Deployment and Inventory
- Installed VirtualBox Guest Additions for improved VM performance.  
![Guest Additions](./screenshots/pdq/guest-additions.png)

- Installed PDQ Deploy to distribute software packages to clients.  
![PDQ Deploy](./screenshots/pdq/deploy.png)

- Used PDQ Inventory to collect and analyze asset data.  
![PDQ Inventory](./screenshots/pdq/inventory.png)

- Deployed and verified software installations across multiple machines.  
![Deployment Success](./screenshots/pdq/deploy-success.png)

---

### 7. Printer and Device Management
- Installed and configured a network printer.  
![Printer Setup](./screenshots/printers/printer-setup.png)

- Added the printer to Active Directory.  
![Printer in AD](./screenshots/printers/printer-ad.png)

- Deployed the printer to client computers using Group Policy.  
![Printer on Client](./screenshots/printers/printer-client.png)

---

### 8. Help Desk Operations
- Reset passwords, unlocked accounts, and rejoined machines to the domain when needed.  
![Account Reset](./screenshots/helpdesk/account-reset.png)

- Enabled and disabled accounts as part of user lifecycle management.  
![Account Disabled](./screenshots/helpdesk/disable-account.png)

- Used Spiceworks to create, assign, and close IT tickets with documentation.  
![Spiceworks Ticket](./screenshots/helpdesk/spiceworks-ticket.png)

- Practiced incident resolution workflows to simulate real-world IT support.  
![Ticket Workflow](./screenshots/helpdesk/ticket-workflow.png)

- Used the Account Lockout Tool to diagnose and resolve locked accounts.  
![Account Lockout Tool](./screenshots/helpdesk/lockout-tool.png)

---

## Commands and Scripts Used

```cmd
# Display network configuration
ipconfig

# Flush DNS
ipconfig /flushdns

# Lists your active network connections
net use

# Account detailes
net user username /domain

# Test connectivity to the server
ping <server-ip>

# Open Task Manager
taskmgr

# Force Group Policy update
gpupdate /force

# Export applied policies
gpresult /r > C:\results.txt

# Map a network drive
net use Z: \\server\HR_Share
```

---

## Skills Demonstrated

- Building and managing enterprise IT infrastructure
- Active Directory administration and OU design
- Group Policy configuration and enforcement
- User and computer account lifecycle management
- File sharing, permissions, and security group management
- Remote administration and troubleshooting
- Enterprise software deployment and inventory management
- Help desk operations and ticketing system workflows

---

## Contact

For any questions you can contact me here:

- LinkedIn: https://www.linkedin.com/in/antonio-karadenizov-37113b289/
