# Incident Response

## Overview

The Incident Response documentation defines the standard procedures used to investigate, analyze, contain, eradicate, and recover from security incidents detected within the Enterprise Detection & Threat Hunting Platform.

These procedures are based on Microsoft Sentinel alerts generated from Windows Security Events and Sysmon telemetry collected through Azure Monitor Agent (AMA). The documentation provides a structured workflow to ensure security incidents are handled consistently and efficiently.

---

## Objectives

- Standardize the incident handling process.
- Improve investigation consistency.
- Minimize response time.
- Preserve investigation evidence.
- Support accurate incident documentation.
- Reduce the impact of security incidents.

---

## Incident Response Lifecycle

The incident response process follows six major phases:

1. Preparation
2. Identification
3. Containment
4. Eradication
5. Recovery
6. Lessons Learned

---

## Documentation

| Document | Description |
|----------|-------------|
| Incident-Classification.md | Defines incident severity levels and classification criteria. |
| Investigation-Workflow.md | Describes the investigation process followed after an alert is generated. |
| Response-Procedure.md | Documents containment, eradication, recovery, and post-incident activities. |

---

## Data Sources

- Microsoft Sentinel
- Azure Log Analytics Workspace
- Windows Security Events
- Sysmon
- Active Directory

---

## Scope

The incident response process supports investigations involving:

- Failed Authentication Attempts
- Account Lockouts
- Privileged Account Activity
- Suspicious Process Creation
- Network Connections
- DNS Queries
- Registry Modifications
- File Creation Events

---

## Purpose

This documentation provides a repeatable and structured incident response methodology that aligns with enterprise SOC operations and supports efficient investigation and remediation of security incidents.
