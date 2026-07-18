# Suspicious Network Connection Investigation Runbook

## Purpose

Investigate suspicious outbound or inbound network connections that may indicate command-and-control (C2) communication, lateral movement, or unauthorized network activity.

## Detection Source

- Microsoft Sentinel
- Sysmon Event ID: 3

## Investigation Steps

1. Review the Microsoft Sentinel alert.
2. Identify the source computer and user.
3. Examine the destination IP address and port.
4. Verify the process responsible for the connection.
5. Determine whether the destination is trusted.
6. Correlate with related process creation and authentication events.

## Evidence Collection

- Sysmon Event ID 3
- Source Computer
- Destination IP
- Destination Port
- Process Name
- User Account

## Containment

- Block malicious IP addresses.
- Isolate affected systems if compromise is confirmed.
- Terminate malicious network activity.

## Recovery

- Remove malicious software.
- Restore normal network connectivity.
- Verify no additional suspicious connections exist.

## Lessons Learned

Review firewall rules, network monitoring, and detection logic to improve future visibility.
