# Disaster Recovery Incident #001

## Date
2026-06-29

## Incident
Host system crashed due to CPU instability while VMware VMs were running.

## Impact
- FG-DC01 entered Automatic Repair.
- FG-CL01 lost its trust relationship with the domain.

## Recovery
- Restored FG-DC01 from the "ADDS Installed" VMware snapshot.
- Re-promoted the Domain Controller.
- Verified DNS, SYSVOL, and NETLOGON.
- Rejoined FG-CL01 to the domain.

## Lessons Learned
- Create VMware snapshots before every major infrastructure change.
- Maintain multiple Domain Controllers.
- Validate host stability before lab work.