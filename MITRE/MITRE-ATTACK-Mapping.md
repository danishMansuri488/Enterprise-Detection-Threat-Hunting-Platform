# MITRE ATT&CK Mapping

## Overview

This document maps the implemented Microsoft Sentinel detections and threat hunting queries to the MITRE ATT&CK framework.

| Detection | MITRE Tactic | MITRE Technique | Status |
|----------|--------------|-----------------|--------|
| Failed Logon Detection | Credential Access | T1110 - Brute Force | Implemented |
| Successful Logon Monitoring | Initial Access | T1078 - Valid Accounts | Implemented |
| Account Lockout Detection | Credential Access | T1110 - Brute Force | Implemented |
| Suspicious Process Creation | Execution | T1059 - Command and Scripting Interpreter | Implemented |
| Suspicious Network Connection | Command and Control | T1071 - Application Layer Protocol | Implemented |
| DNS Query Monitoring | Command and Control | T1071.004 - DNS | Implemented |
| File Creation Monitoring | Collection | T1005 - Data from Local System | Implemented |
| Registry Activity Monitoring | Persistence | T1112 - Modify Registry | Implemented |
| Privileged Account Activity | Privilege Escalation | T1078 - Valid Accounts | Implemented |

## Summary

The implemented detections are aligned with the MITRE ATT&CK framework to provide standardized detection coverage and improve investigation workflows.
