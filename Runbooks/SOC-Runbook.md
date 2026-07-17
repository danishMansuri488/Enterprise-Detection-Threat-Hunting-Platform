# SOC Runbook

## Overview

This runbook provides a standardized investigation process for Microsoft Sentinel detections generated in the Enterprise Detection & Threat Hunting Platform.

## Detection Description

Review the alert details, affected assets, analytics rule, severity, and related events.

## Investigation Steps

1. Review the generated alert.
2. Validate related Windows Security Events and Sysmon logs.
3. Identify the affected user and host.
4. Analyze authentication and process activity.
5. Determine whether the activity is malicious or benign.

## Containment

- Isolate the affected endpoint if required.
- Disable or lock compromised user accounts.
- Block malicious activity where appropriate.

## Recovery

- Remove malicious artifacts.
- Restore affected systems.
- Verify that normal operations have resumed.

## Escalation Guidance

Escalate confirmed incidents to the security team when additional investigation or remediation is required.

## Closure Procedure

- Document findings.
- Record root cause.
- Update detection logic if necessary.
- Close the incident after verification.
