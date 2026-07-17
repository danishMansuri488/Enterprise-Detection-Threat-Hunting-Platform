# File Creation Monitoring

## Purpose
Detect file creation events that may indicate unauthorized file modifications or malicious activity.

## Data Source
- Sysmon Operational Logs

## Event ID
- 11 (File Create)

## MITRE ATT&CK
- T1105 – Ingress Tool Transfer

## Detection Logic
Monitor Sysmon File Creation events to identify newly created files in monitored systems that may be associated with suspicious activity.

## Investigation Steps
- Review the file name and file path.
- Identify the creating process.
- Verify the user account responsible.
- Determine whether the file creation is legitimate or suspicious.

## Expected Outcome
Generate a Microsoft Sentinel incident for suspicious file creation requiring analyst investigation.
