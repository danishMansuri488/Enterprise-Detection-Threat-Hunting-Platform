# DNS Query Investigation Runbook

## Purpose

Investigate suspicious DNS queries that may indicate command-and-control (C2) communication, domain generation algorithms (DGA), or connections to malicious domains.

## Detection Source

- Microsoft Sentinel
- Sysmon Event ID: 22

## Investigation Steps

1. Review the Microsoft Sentinel alert.
2. Identify the queried domain name.
3. Verify the process that initiated the DNS request.
4. Determine the affected user and host.
5. Check whether the domain is known to be malicious or suspicious.
6. Correlate with related network connection events and process activity.

## Evidence Collection

- Sysmon Event ID 22
- Queried Domain
- Process Name
- User Account
- Host Information
- Timestamp

## Containment

- Block malicious domains through DNS or firewall controls.
- Isolate affected systems if compromise is confirmed.
- Stop malicious processes generating DNS traffic.

## Recovery

- Remove malicious software.
- Validate normal DNS activity after remediation.
- Monitor for recurring suspicious queries.

## Lessons Learned

Update threat intelligence, detection logic, and monitoring rules based on investigation findings.
