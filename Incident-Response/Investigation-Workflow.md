# Investigation Workflow

## Overview

This document defines the standard investigation workflow followed by Security Operations Center (SOC) analysts after a Microsoft Sentinel alert is generated. The objective is to validate alerts, determine the scope of impact, collect evidence, and perform appropriate response actions.

---

## Investigation Workflow

### 1. Alert Validation

- Review the Microsoft Sentinel incident.
- Identify the triggered analytics rule.
- Verify the alert severity and affected assets.
- Confirm that the alert is not a false positive.

---

### 2. Initial Triage

Collect key information including:

- Timestamp
- Hostname
- User Account
- Source IP Address
- Event ID
- Process Name (if applicable)
- Alert Description

---

### 3. Evidence Collection

Collect relevant security evidence from:

- Microsoft Sentinel
- Azure Log Analytics Workspace
- Windows Security Events
- Sysmon
- Active Directory

---

### 4. Correlation Analysis

Correlate the alert with related security events to determine the full attack scope.

Examples include:

- Failed and successful logons
- Account lockouts
- Process creation events
- Network connections
- DNS queries
- Registry modifications

---

### 5. Incident Assessment

Determine:

- Impacted systems
- Affected user accounts
- Privilege level
- Potential attacker objectives
- MITRE ATT&CK techniques involved

---

### 6. Response Decision

Based on the investigation, determine whether to:

- Close as False Positive
- Continue Monitoring
- Escalate for Incident Response
- Begin Containment

---

## Investigation Outcome

Every investigation should conclude with:

- Incident classification
- Root cause
- Evidence summary
- Response actions performed
- Lessons learned

---

## Purpose

This workflow ensures investigations are performed consistently, efficiently, and in accordance with standard SOC operational practices.
