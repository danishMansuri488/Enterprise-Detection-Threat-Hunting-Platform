# Suspicious Process Creation Investigation Runbook

## Purpose

Investigate suspicious process creation events that may indicate malicious execution, command-line abuse, or attacker activity.

## Detection Source

- Microsoft Sentinel
- Sysmon Event ID: 1

## Investigation Steps

1. Review the Microsoft Sentinel alert.
2. Identify the process name and full command line.
3. Verify the parent process.
4. Determine which user executed the process.
5. Check whether the process is legitimate or suspicious.
6. Correlate with related Sysmon and Windows Security Events.

## Evidence Collection

- Sysmon Event ID 1
- Process Name
- Command Line
- Parent Process
- User Account
- Host Information

## Containment

- Terminate malicious processes.
- Isolate the affected endpoint if necessary.
- Block malicious executables.

## Recovery

- Remove malicious files.
- Perform endpoint malware scanning.
- Verify that no unauthorized processes remain.

## Lessons Learned

Update detection rules and investigation procedures based on findings.
