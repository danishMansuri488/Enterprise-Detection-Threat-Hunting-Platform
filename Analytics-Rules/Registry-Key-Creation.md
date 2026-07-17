# Registry Key Creation

## Purpose
Detect the creation of new registry keys that may indicate persistence or unauthorized system modifications.

## Data Source
- Sysmon Operational Logs

## Event ID
- 12 (Registry Object Create/Delete)

## MITRE ATT&CK
- T1112 – Modify Registry

## Detection Logic
Monitor Sysmon Registry events to identify newly created registry keys that may be associated with persistence or malicious activity.

## Investigation Steps
- Review the registry key path.
- Identify the process responsible.
- Verify the user account.
- Determine whether the registry modification is legitimate or suspicious.

## Expected Outcome
Generate a Microsoft Sentinel incident for suspicious registry key creation requiring analyst investigation.
