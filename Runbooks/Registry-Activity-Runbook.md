# Registry Activity Investigation Runbook

## Purpose

Investigate suspicious Windows Registry modifications that may indicate persistence, privilege escalation, or malicious system configuration changes.

## Detection Source

- Microsoft Sentinel
- Sysmon Event IDs: 12, 13

## Investigation Steps

1. Review the Microsoft Sentinel alert.
2. Identify the modified registry key or value.
3. Determine the process responsible for the modification.
4. Verify the affected user account and endpoint.
5. Assess whether the registry change is authorized.
6. Correlate with related process creation and authentication events.

## Evidence Collection

- Sysmon Event IDs 12 and 13
- Registry Path
- Modified Value
- Process Name
- User Account
- Host Information
- Timestamp

## Containment

- Revert unauthorized registry changes.
- Terminate malicious processes.
- Isolate the affected endpoint if required.

## Recovery

- Restore legitimate registry configuration.
- Perform malware scanning.
- Validate normal system operation.

## Lessons Learned

Review registry monitoring rules and strengthen detection coverage for persistence techniques.
