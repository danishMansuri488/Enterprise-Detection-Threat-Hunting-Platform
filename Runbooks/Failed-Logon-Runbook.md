# Failed Logon Investigation Runbook

## Purpose

Investigate repeated failed authentication attempts that may indicate brute-force attacks, password spraying, or invalid credential usage.

## Detection Source

- Microsoft Sentinel
- Windows Security Event ID: 4625

## Investigation Steps

1. Review the alert details in Microsoft Sentinel.
2. Identify the affected user account.
3. Verify the source computer and IP address.
4. Check the number of failed attempts.
5. Determine whether the activity is expected or suspicious.
6. Correlate with successful logon events (Event ID 4624).

## Evidence Collection

- SecurityEvent (4625)
- Related authentication events
- Source host information

## Containment

- Lock or disable compromised accounts if required.
- Block malicious source systems when applicable.

## Recovery

- Reset affected credentials.
- Verify successful authentication after remediation.

## Lessons Learned

Review detection logic and improve monitoring based on investigation findings.
