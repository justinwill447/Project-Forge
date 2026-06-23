## Purpose

This document defines the network architecture for Forge Technologies.

The architecture is designed to support 150 employees while providing scalability, security, and operational efficiency for future growth.

## Network Address Space

Primary Network:

10.10.0.0/16

Subnet Mask:

255.255.0.0

## Planned Infrastructure

Domain Controllers: 2

File Servers: 1

Monitoring Servers: 1

Security Servers: 2

Client Systems: 150+

Cloud Services: Microsoft 365, AWS

## VLAN Design

| VLAN | Purpose | Network |
|--------|--------|--------|
| VLAN 10 | Servers | 10.10.10.0/24 |
| VLAN 20 | Workstations | 10.10.20.0/24 |
| VLAN 30 | Network Devices | 10.10.30.0/24 |
| VLAN 40 | Management | 10.10.40.0/24 |
| VLAN 50 | Security Tools | 10.10.50.0/24 |
| VLAN 60 | Remote Access VPN | 10.10.60.0/24 |

## Default Gateways

VLAN 10 - 10.10.10.1

VLAN 20 - 10.10.20.1

VLAN 30 - 10.10.30.1

VLAN 40 - 10.10.40.1

VLAN 50 - 10.10.50.1

VLAN 60 - 10.10.60.1

## Server Network

Server VLAN:

VLAN 10

Network:

10.10.10.0/24

Planned Systems:

FG-DC01

FG-DC02

FG-FS01

FG-WEB01

FG-APP01

FG-MON01

## Workstation Network

Workstation VLAN:

VLAN 20

Network:

10.10.20.0/24

Supported Systems:

Employee Workstations

Administrative Workstations

Remote User Devices

## Security Network

Security VLAN:

VLAN 50

Planned Systems:

Splunk

Wazuh

Security Onion

Future Security Monitoring Tools

## Remote Access Strategy

Forge Technologies supports hybrid and remote workers.

Remote connectivity shall be provided through VPN services.

Future Implementation:

pfSense VPN

Microsoft Entra Integration

Multi-Factor Authentication

## Cloud Integration

Cloud Providers:

Microsoft 365

Microsoft Entra ID

Amazon Web Services (AWS)

Future Goals:

Hybrid Identity

Cloud Backups

Cloud Monitoring

Disaster Recovery

## Security Principles

- Least Privilege Access

- Network Segmentation

- Multi-Factor Authentication

- Centralized Logging

- Security Monitoring

- Regular Backups

- Change Management

## Network Diagram

Diagram Pending Development

## Lessons Learned

Network architecture should be designed before systems are deployed.

Proper segmentation improves security, scalability, and troubleshooting efficiency.

## Revision History

| Version | Date | Change |
|----------|----------|----------|
| 1.0 | 2026-06-23 | Initial network architecture design |

