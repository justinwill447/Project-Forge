# Ticket #0013 — Forge Workstation Group Policy Baseline

## Status
Completed

## Objective

Implement a centrally managed security baseline for Windows workstations in the Forge Technologies Active Directory environment.

## Environment

- Domain: forge.local
- Domain Controller: FG-DC01
- Client Workstation: FG-CL01
- Target OU: Forge Technologies/Workstations
- Group Policy Object: Forge Workstation Baseline

## Implementation

A new Group Policy Object named `Forge Workstation Baseline` was created and linked directly to the `Workstations` Organizational Unit.

The policy was scoped to the Workstations OU to ensure that workstation-specific security settings are applied to domain-joined client systems without affecting domain controllers or servers.

## Security Settings Configured

### Interactive Logon

- Authorized-use legal notice configured
- Last signed-in username hidden
- Ctrl+Alt+Delete required for secure sign-in
- Machine inactivity limit configured for 900 seconds

### Windows Defender Firewall

Windows Defender Firewall was enabled for:

- Domain Profile
- Private Profile
- Public Profile

Default firewall behavior was maintained:

- Inbound connections: Block
- Outbound connections: Allow

## Validation

The policy was applied to FG-CL01 using:

`gpupdate /force`

Both Computer Policy and User Policy completed successfully.

Policy application was verified using:

`gpresult /r /scope computer`

The results confirmed that `Forge Workstation Baseline` was listed under Applied Group Policy Objects.

After restarting FG-CL01, the configured Forge Technologies authorized-access notice was successfully displayed before user sign-in.

The workstation successfully authenticated to the forge.local domain after the policy was applied.

## Result

The Forge Technologies environment now has a centrally managed workstation security baseline that can automatically apply standardized security settings to computers placed within the Workstations OU.

## Lessons Learned

- Group Policy links determine where policies are applied within Active Directory.
- Workstation-specific policies should be scoped to workstation OUs rather than the entire domain.
- `gpupdate /force` can be used to immediately refresh Group Policy.
- `gpresult` provides evidence of which Group Policy Objects were successfully applied.
- A legal logon notice provides a clear visual method for validating successful computer-side Group Policy processing.

## Evidence

- Workstation GPO linked to the Workstations OU
- Configured workstation security settings
- `gpresult` showing successful GPO application
- Authorized-access notice displayed on FG-CL01