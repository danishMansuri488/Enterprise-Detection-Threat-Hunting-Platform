# Incident Classification

## Overview

Incident classification provides a standardized method for prioritizing security incidents based on their potential impact, affected assets, and urgency. Proper classification enables Security Operations Center (SOC) analysts to respond consistently and allocate resources effectively.

---

## Severity Levels

| Severity | Description | Example |
|----------|-------------|---------|
| Critical | Active compromise or significant business impact requiring immediate response. | Domain Admin compromise, ransomware, confirmed malware outbreak |
| High | Confirmed malicious activity affecting important systems or privileged accounts. | Privileged account misuse, lateral movement, persistence |
| Medium | Suspicious activity requiring investigation with moderate business impact. | Brute-force attacks, multiple account lockouts, suspicious process execution |
| Low | Low-risk or isolated events with minimal operational impact. | Single failed login, policy violations |
| Informational | Events recorded for monitoring purposes with no immediate security risk. | Successful authentication, routine administrative actions |

---

## Classification Factors

Incident severity is determined using the following criteria:

- Business impact
- Criticality of affected assets
- Number of affected systems
- Privilege level of impacted accounts
- Evidence of compromise
- Potential for lateral movement
- Data confidentiality and integrity risks

---

## Priority Matrix

| Severity | Response Priority | Target Response |
|----------|-------------------|-----------------|
| Critical | P1 | Immediate |
| High | P2 | High Priority |
| Medium | P3 | Standard Investigation |
| Low | P4 | Routine Review |
| Informational | P5 | Monitoring Only |

---

## Purpose

A standardized incident classification process improves response consistency, reduces investigation time, and ensures security resources are focused on the highest-risk incidents.
