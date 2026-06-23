## Host System

Windows 11 Pro
Intel i9 14th Gen
64 GB RAM
Samsung 990 Pro 2TB
Seagate 8TB HDD

## Hypervisor Selection

Selected Hypervisor:
VMware Workstation Pro

Reasoning:

VMware Workstation Pro was selected as the primary hypervisor for Project Forge due to its enterprise adoption, stability, networking capabilities, snapshot management, and alignment with real-world corporate IT environments.

While VirtualBox offers excellent flexibility and open-source advantages, VMware provides a more realistic enterprise experience that directly supports the goals of Forge Technologies.

## Initial VM Inventory

FG-DC01
Primary Domain Controller

Windows Server 2025
4 GB RAM
2 vCPU
80 GB Disk

FG-DC02
Secondary Domain Controller

Windows Server 2025
4 GB RAM
2 vCPU
80 GB Disk

FG-FS01
File Server

Windows Server 2025
4 GB RAM
2 vCPU
100 GB Disk

FG-CL01
Windows 11 Client

4 GB RAM
2 vCPU
60 GB Disk

FG-KALI01
Kali Linux

4 GB RAM
2 vCPU
60 GB Disk

## Network Design

Forge-Server-Network

Used for:
- Domain Controllers
- File Servers
- Infrastructure Services

Forge-Client-Network

Used for:
- Employee Workstations
- Administrative Systems

Forge-Security-Network

Used for:
- Splunk
- Wazuh
- Security Monitoring Systems

## Lessons Learned

Planning virtual infrastructure before deployment helps ensure efficient resource allocation, scalability, and maintainability throughout the project lifecycle.

## Revision History

| Version | Date | Change |
|----------|----------|----------|
| 1.0 | 2026-06-23 | Initial virtual infrastructure design |