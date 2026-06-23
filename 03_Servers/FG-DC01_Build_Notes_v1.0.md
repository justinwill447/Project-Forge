# FG-DC01 Build Notes

Version: 1.0

Server Name:
FG-DC01

Purpose:
Primary Domain Controller

Operating System:
Windows Server 2025

Deployment Status:
Not Started

Planned Resources:

RAM:
4096 MB

CPU:
2 vCPU

Disk:
80 GB

Network:
NAT (Initial Deployment)

Build Date: 
Pending

## Server Identity

Hostname:
FG-DC01

Operating System:
Windows Server 2025

Initial DHCP Address:
192.168.238.128

Assigned Static Address:
192.168.238.10

Gateway:
192.168.238.2

## Active Directory Domain Services

Installation Status:
Installed

Promotion Status:
Pending

Snapshot Created:
FG-DC01 - ADDS Installed

## Domain Promotion

Domain Name:
forge.local

NetBIOS Name:
FORGE

Promotion Status:
Completed

DNS:
Installed

Global Catalog:
Enabled

Promotion Date:
2026-06-23

## Issues Encountered

VMware displayed a warning indicating that Virtualized Intel VT-x/EPT was not supported.

Root Cause:
Nested virtualization was enabled in VM processor settings.

Resolution:
Disabled Virtualize Intel VT-x/EPT and Virtualize IOMMU under Processor settings.

Outcome:
VM booted successfully.

Notes:

Lessons Learned:

Revision History:

| Version | Date | Change |
|----------|----------|----------|
| 1.0 | 2026-06-23 | Initial build document created |