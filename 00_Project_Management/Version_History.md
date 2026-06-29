# Project Forge Version History

---

## v0.1 - Virtual Infrastructure

### Completed
- VMware Workstation installed
- Virtual networking configured
- FG-DC01 created
- FG-CL01 created

Status:
✅ Complete

---

## v0.2 - Windows Server

### Completed
- Windows Server 2025 installed
- Static IP configured
- VMware Tools installed

Status:
✅ Complete

---

## v0.3 - Active Directory

### Completed
- AD DS installed
- Domain Controller promoted
- DNS configured

Status:
✅ Complete

---

## v0.4 - Workstation Deployment

### Completed
- Windows 11 installed
- Joined FG-CL01 to forge.local

Status:
✅ Complete

---

## Recovery Incident #001

Cause:
Host CPU instability caused VMware guests to shut down unexpectedly.

Recovery:
- Restored VMware snapshot
- Re-promoted Domain Controller
- Verified DNS
- Verified SYSVOL
- Verified NETLOGON
- Rejoined FG-CL01

Lessons Learned:
- Snapshot before every major change
- Snapshot after every successful ticket
- Build redundant Domain Controllers