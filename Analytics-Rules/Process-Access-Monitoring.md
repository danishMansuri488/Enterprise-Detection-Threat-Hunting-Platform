# Process Access Monitoring

## Purpose
Detect suspicious process access events that may indicate credential dumping or unauthorized access to sensitive processes.

## Data Source
- Sysmon Operational Logs

## Event ID
- 10 (Process Access)

## MITRE ATT&CK
- T1003 – OS Credential Dumping

## Detection Logic
Monitor Sysmon Process Access events to identify processes attempting to access sensitive system or security-related processes.

## Investigation Steps
- Review the source process.
- Identify the target process.
- Verify the access permissions requested.
- Determine whether the activity is legitimate or suspicious.

## Expected Outcome
Generate a Microsoft Sentinel incident for suspicious process access requiring analyst investigation.
