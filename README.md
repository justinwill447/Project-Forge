# 🏢 Project Forge

> A hands-on enterprise Windows infrastructure lab designed to simulate a real-world corporate IT environment.

![Status](https://img.shields.io/badge/Status-Operational-brightgreen)
![Version](https://img.shields.io/badge/Version-v0.4-blue)
![Platform](https://img.shields.io/badge/Platform-VMware_Workstation-orange)
![Windows](https://img.shields.io/badge/Windows_Server-2025-success)

---

# 📖 Overview

Project Forge is an enterprise infrastructure lab built to develop and demonstrate practical systems administration skills. The environment simulates a small-to-medium business running Microsoft Active Directory and Windows Server.

The goal of this project is to gain real-world experience with enterprise technologies including:

* Active Directory Domain Services
* DNS
* Group Policy
* Windows Server Administration
* Windows 11 Enterprise
* VMware Virtualization
* PowerShell Automation
* Disaster Recovery
* Security Hardening
* Enterprise Documentation

Every change to the environment is documented through tickets, build notes, version history, and change logs to mirror professional IT operations.

---

# 🎯 Project Goals

* Build an enterprise Active Directory environment
* Practice Windows Server administration
* Learn enterprise networking concepts
* Develop PowerShell automation skills
* Implement security best practices
* Simulate real-world help desk scenarios
* Create professional documentation suitable for a technical portfolio

---

# 🏢 Simulated Company

**Company Name**

Forge Technologies

**Industry**

Technology Services

**Environment Size**

* 1 Domain
* Windows Server 2025
* Windows 11 Enterprise Clients
* VMware Workstation Pro
* Private Virtual Network

---

# 🖥️ Current Infrastructure

## Domain

```
forge.local
```

## Domain Controller

| Server  | Role                  |
| ------- | --------------------- |
| FG-DC01 | Active Directory, DNS |

## Workstations

| Computer | Operating System      |
| -------- | --------------------- |
| FG-CL01  | Windows 11 Enterprise |

---

# 📂 Active Directory Structure

```
Forge Technologies
│
├── Users
├── Groups
├── Computers
├── Servers
├── Workstations
├── Cybersecurity
├── IT
├── Finance
├── HR
└── Executive
```

---

# 🔐 Security Groups

Current security groups include:

* GG_IT_Admins
* GG_Cybersecurity
* GG_HR
* GG_Finance
* GG_Executives
* GG_Workstations

---

# 🛠️ Technologies

* Windows Server 2025
* Windows 11 Enterprise
* VMware Workstation Pro
* Active Directory Domain Services
* DNS
* Group Policy
* PowerShell
* Git
* GitHub
* Visual Studio Code

---

# 📋 Current Progress

## Completed

* VMware environment
* Windows Server deployment
* Active Directory deployment
* DNS configuration
* Windows 11 client deployment
* Domain join
* Active Directory organizational structure
* Security groups
* Enterprise documentation

---

## In Progress

* Enterprise Group Policy Baseline

---

## Planned

* File Server
* NTFS Permissions
* DHCP
* Windows Server Update Services (WSUS)
* Windows Event Forwarding
* PowerShell Automation
* Security Hardening
* Second Domain Controller
* Microsoft Entra ID Hybrid Lab

---

# 🚨 Disaster Recovery

Project Forge experienced an unexpected host system crash that corrupted the Domain Controller.

Recovery actions included:

* Windows Recovery Environment troubleshooting
* Offline CHKDSK
* Offline SFC
* Offline DISM
* VMware Snapshot restoration
* Active Directory recovery
* Domain rejoin of client workstation

This incident reinforced the importance of virtualization snapshots, documentation, and disaster recovery planning.

---

# 📚 Documentation

Project documentation includes:

* Infrastructure Design
* Active Directory Design
* Network Architecture
* Build Notes
* Disaster Recovery Reports
* Infrastructure Standards
* Change Logs
* Version History
* Ticket Tracking

---

# 🚀 Roadmap

Upcoming milestones include:

* Enterprise Group Policy
* File Server
* DFS
* WSUS
* DHCP
* Security Hardening
* SIEM Integration
* Windows Event Forwarding
* Microsoft Entra ID Hybrid Environment

---

# 📈 Current Version

```
v0.4
```

Status:

🟢 Operational

---

# 👨‍💻 Author

**Justin Willadsen**

Project Forge is an ongoing enterprise systems administration lab created to strengthen hands-on experience with Microsoft infrastructure, virtualization, automation, and cybersecurity technologies.
