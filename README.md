# Enterprise IT Lab Environment

This project showcases the design and administration of a **simulated corporate IT infrastructure** built with **Windows Server 2022, Active Directory, Group Policy, Windows 10 Pro clients, and enterprise IT management tools**.  

The lab demonstrates the ability to plan, configure, and maintain a domain-based environment, enforce security standards, deploy software, and handle real-world help desk scenarios. It reflects the skill set required of a **Systems Administrator / IT Support Specialist** in an enterprise setting.

---

## Project Objectives
- Build a virtualized **enterprise network environment**
- Demonstrate **Active Directory domain management** and **Group Policy administration**
- Show proficiency in **user/computer lifecycle management**
- Configure **enterprise security policies**
- Deploy and inventory software with **PDQ**
- Perform **remote administration and troubleshooting**
- Simulate **help desk workflows** with Spiceworks

---

## Lab Environment
- **Hypervisor:** VirtualBox  
- **Server:** Windows Server 2022 (Domain Controller)  
- **Clients:** Windows 10 Pro (multiple departmental machines: IT, HR)  
- **Management Tools:** RSAT, PDQ Deploy, PDQ Inventory, Spiceworks, Account Lockout Tool  

---

## Project Phases

### 1. Infrastructure Setup
- Installed and configured Windows Server 2022  
- Installed Active Directory Domain Services (AD DS)  
- Configured static IP addresses for server and clients  
- Joined Windows 10 clients to the domain  
- Verified connectivity using `ping`  

---

### 2. Active Directory & User Management
- Created and managed **Organizational Units (OUs)** for IT, HR, and Helpdesk  
- Created and managed user/computer accounts  
- Enabled AD Recycle Bin for recovery  
- Delegated control to specific groups  
- Reset/unlocked accounts, enabled/disabled accounts  

---

### 3. Policy & Security Management
- Configured Group Policy Objects (GPOs) for:  
  - Password complexity, history, and expiration  
  - Account lockout thresholds and timeouts  
  - Disabling system features (e.g., Task Manager, Logoff option)  
- Verified enforcement using `gpresult /r` and `gpupdate /force`  

---

### 4. File Sharing & Drive Management
- Created **shared network drives** with NTFS and share permissions  
- Mapped drives via Active Directory and client-side configuration  
- Created **security groups** for access control  

---

### 5. Remote Administration
- Performed remote desktop connections and Windows Remote Assistance  
- Accessed administrative shares (`C$`) for user file management  
- Remotely accessed the Registry  

---

### 6. Software Deployment & Inventory
- Installed and configured **PDQ Deploy** for software rollouts  
- Used **PDQ Inventory** for asset management and reporting  
- Deployed applications to multiple domain-joined clients  

---

### 7. Printer & Device Management
- Installed and shared a network printer  
- Added printer objects to Active Directory  
- Deployed printers to client machines via GPO  

---

### 8. Help Desk Operations
- Used **Spiceworks** for ticketing:  
  - Created, assigned, resolved, and documented tickets  
- Practiced **IT support scenarios**:  
  - Password resets  
  - Account unlocks  
  - Rejoining machines to the domain  

---

## Tools & Technologies
- **Server OS:** Windows Server 2022  
- **Client OS:** Windows 10 Pro  
- **Directory Services:** Active Directory (AD DS)  
- **Policy Management:** Group Policy Objects (GPO)  
- **Administration Tools:** RSAT, CMD, PowerShell  
- **Deployment & Inventory:** PDQ Deploy, PDQ Inventory  
- **Help Desk:** Spiceworks  
- **Support Tools:** Account Lockout Tool  

---

## Skills Demonstrated
- Enterprise network infrastructure design  
- Domain and user/computer account management  
- Group Policy configuration and enforcement  
- File sharing and permission management  
- Remote administration and troubleshooting  
- Software deployment and IT asset inventory  
- Help desk operations and customer support workflows  

---

## Evidence of Work
All major steps are documented through **screenshots, commands, and configurations**, stored in:  
- `/screenshots` → Server, AD, GPOs, PDQ, Spiceworks  
- `/scripts` → PowerShell and CMD snippets  
- `/docs` → Network diagram and additional notes  

---

## Future Enhancements
- Automate user and group management with PowerShell scripts  
- Expand to multi-site Active Directory with replication  
- Integrate Linux/Mac clients into the domain  
- Centralize monitoring with enterprise logging tools  

---

## Contact
If you’d like to discuss this project or my IT administration experience:  
- **LinkedIn:** [Your LinkedIn Profile]  
- **Email:** [Your Email]  
