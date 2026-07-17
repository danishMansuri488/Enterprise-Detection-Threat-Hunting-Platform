# Detection Quality Metrics

## Overview

This document tracks the quality and validation status of detections implemented in the Enterprise Detection & Threat Hunting Platform.

| Detection | Version | Severity | Data Source | MITRE Technique | Validation Status | Tuning Status |
|-----------|---------|----------|-------------|-----------------|-------------------|---------------|
| Failed Logon Detection | 1.0 | Medium | Windows Security Events | T1110 | Validated | Complete |
| Successful Logon Monitoring | 1.0 | Low | Windows Security Events | T1078 | Validated | Complete |
| Account Lockout Detection | 1.0 | High | Windows Security Events | T1110 | Validated | Complete |
| Suspicious Process Creation | 1.0 | High | Sysmon | T1059 | Validated | Complete |
| Suspicious Network Connection | 1.0 | Medium | Sysmon | T1071 | Validated | Complete |
| DNS Query Monitoring | 1.0 | Medium | Sysmon | T1071.004 | Validated | Complete |
| File Creation Monitoring | 1.0 | Medium | Sysmon | T1005 | Validated | Complete |
| Registry Activity Monitoring | 1.0 | Medium | Sysmon | T1112 | Validated | Complete |
| Privileged Account Activity | 1.0 | High | Windows Security Events | T1078 | Validated | Complete |
