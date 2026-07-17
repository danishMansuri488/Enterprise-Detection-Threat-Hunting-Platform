# Suspicious Process Creation

## Purpose
Detect suspicious process creation events that may indicate malicious activity on Windows endpoints.

## Data Source
- Sysmon Operational Logs

## Event ID
- 1 (Process Create)

## MITRE ATT&CK
- T1059 – Command and Scripting Interpreter

## Detection Logic
Monitor Sysmon Process Creation events to identify suspicious or unauthorized processes executed on monitored systems.

## Investigation Steps
- Review the process name.
- Verify the parent process.
- Check the command line arguments.
- Determine whether the process is legitimate or malicious.

## Expected Outcome
Generate a Microsoft Sentinel incident for suspicious process execution requiring analyst investigation.
