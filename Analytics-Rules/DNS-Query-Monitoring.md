# DNS Query Monitoring

## Purpose
Monitor DNS query activity to identify communication with suspicious or unauthorized domains.

## Data Source
- Sysmon Operational Logs

## Event ID
- 22 (DNS Query)

## MITRE ATT&CK
- T1071.004 – Application Layer Protocol: DNS

## Detection Logic
Monitor Sysmon DNS Query events to identify unusual domain requests that may indicate command-and-control (C2) communication or malicious activity.

## Investigation Steps
- Review the queried domain.
- Verify the requesting process.
- Check the frequency of DNS requests.
- Determine whether the domain is trusted or suspicious.

## Expected Outcome
Generate a Microsoft Sentinel incident for suspicious DNS activity requiring analyst investigation.
