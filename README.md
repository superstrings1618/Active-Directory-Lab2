>> 🔬 Hands-on Active Directory lab simulating real-world IT Analyst tasks:
> domain setup, DNS troubleshooting, Group Policy, and Windows 11 client onboarding.

# Active Directory Lab 2
## Objective
...
🔹 Title
# Active-Directory-Lab2
# Active Directory Lab 2 – Domain, DNS, GPO, and Client Join
🔹 Objective
The goal of this lab was to design, configure, and troubleshoot a Windows Active Directory
environment including Domain Services, DNS, Organizational Units (OUs),
Group Policy Objects (GPOs), and a Windows 11 domain-joined client.
This lab simulates real-world IT Analyst and System Administrator tasks such as
user management, workstation onboarding, DNS troubleshooting, and policy enforcement.
🔹 Objective
## Lab Environment
- Hypervisor: Oracle VirtualBox
- Domain Controller: Windows Server (AD DS + DNS)
- Client Machine: Windows 11
- Network Type: Internal Network
- Domain Name: lab.local
🔹 Network Configuration
## Network Configuration

Domain Controller:
- IP Address: 192.168.100.10
- Subnet Mask: 255.255.255.0
- Default Gateway: 192.168.100.1
- DNS Server: 192.168.100.10

Windows 11 Client:
- Static IP configured in same subnet
- DNS manually set to Domain Controller IP
🔹 Active Directory Structure
## Active Directory Design

Organizational Units (OUs):
- LAB_Users
- LAB_Workstations
- IT_Staff (removed after restructuring)
- HR_Staff (removed after restructuring)

Users:
- jdoe
- ssmith

Computer:
- Windows 11 domain-joined workstation
🔹 Group Policy Management
## Group Policy

- GPMC used to create and manage GPOs
- GPO linked to appropriate OU
- Inheritance behavior tested
- GPO enabled and verified

Purpose:
- Understand policy scope
- Practice enterprise policy control
🔹 Domain Join & Troubleshooting
## Domain Join Process

Steps:
1. Verified DNS resolution to Domain Controller
2. Confirmed network connectivity
3. Joined Windows 11 to the domain
4. Verified computer object creation in ADUC
5. Logged in using domain user credentials

Common Issues Resolved:
- APIPA address (169.254.x.x)
- DNS misconfiguration
- Network adapter mismatch
🔹 Commands Used (High-Level)
## Key Commands Used

Networking:
- ipconfig /all
- ping
- nslookup
- net view

System:
- hostname
- whoami
- gpupdate /force

Purpose:
- Network verification
- Domain connectivity
- Policy refresh
🔹 Key Takeaways
## Key Takeaways

- DNS is critical for Active Directory functionality
- OU design affects security and scalability
- Group Policy must be carefully linked and tested
- Troubleshooting is a core IT Analyst skill
- Documentation is as important as configuration
🔹 Skills Demonstrated
## Skills Demonstrated

- Active Directory Administration
- DNS Troubleshooting
- Windows Client Domain Join
- Group Policy Management
- Virtualized Lab Environments
- IT Documentation
📁 Optional Folder Structure
/screenshots
/configs
/notes
## 📸 LAB 2 – Screenshots

### Domain Controller (DC01)
![DC01 ADUC](screenshots/dc01-aduc.png)
![GPMC](screenshots/gpmc.png)

### Windows 11 Client
![Win11 Domain Join](screenshots/win11-domain-join.png)
![User Login Test](screenshots/win11-jdoe-login.png)

