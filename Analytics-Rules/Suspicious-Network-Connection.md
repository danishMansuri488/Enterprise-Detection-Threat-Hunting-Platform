# Suspicious Network Connection

## Purpose
Detect suspicious outbound and inbound network connections that may indicate malicious communication or unauthorized access.

## Data Source
- Sysmon Operational Logs

## Event ID
- 3 (Network Connection)

## MITRE ATT&CK
- T1071 – Application Layer Protocol

## Detection Logic
Monitor Sysmon Network Connection events to identify unusual or unauthorized network communication from monitored endpoints.

## Investigation Steps
- Review the source and destination IP addresses.
- Verify the destination port and protocol.
- Identify the initiating process.
- Determine whether the connection is legitimate or suspicious.

## Expected Outcome
Generate a Microsoft Sentinel incident for suspicious network activity requiring analyst investigation.
