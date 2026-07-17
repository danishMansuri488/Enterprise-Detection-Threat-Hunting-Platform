# Registry Value Modification

## Purpose
Detect modifications to registry values that may indicate persistence, defense evasion, or unauthorized system configuration changes.

## Data Source
- Sysmon Operational Logs

## Event ID
- 13 (Registry Value Set)

## MITRE ATT&CK
- T1112 – Modify Registry

## Detection Logic
Monitor Sysmon Registry Value Set events to identify unauthorized or suspicious modifications to Windows registry values.

## Investigation Steps
- Review the modified registry value.
- Identify the process responsible.
- Verify the user account.
- Determine whether the modification is legitimate or suspicious.

## Expected Outcome
Generate a Microsoft Sentinel incident for suspicious registry value modifications requiring analyst investigation.
