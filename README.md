# Enterprise Detection & Threat Hunting Platform

> **A production-inspired Microsoft Sentinel SOC project demonstrating Detection Engineering, Threat Hunting, Incident Response, and Active Directory Security Monitoring.**

![Platform](https://img.shields.io/badge/Platform-Microsoft%20Azure-0078D4?style=for-the-badge&logo=microsoftazure)
![SIEM](https://img.shields.io/badge/SIEM-Microsoft%20Sentinel-5E5E5E?style=for-the-badge)
![Language](https://img.shields.io/badge/KQL-Kusto%20Query%20Language-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

---

# 📖 Project Overview

This project simulates an enterprise Security Operations Center (SOC) using Microsoft Sentinel to detect, investigate, and respond to security events across Windows endpoints and an Active Directory environment.

Windows Security Events and Sysmon telemetry are collected through Azure Monitor Agent (AMA) and centralized in Azure Log Analytics Workspace. Microsoft Sentinel is used to develop custom Analytics Rules, perform proactive threat hunting with Kusto Query Language (KQL), investigate incidents, and validate detections through attack simulation.

The project demonstrates a complete Detection Engineering lifecycle—from log collection and detection development to incident investigation and documentation.

---

# ✨ Key Features

- Enterprise-inspired Microsoft Sentinel deployment
- Active Directory security monitoring
- Windows Security Event and Sysmon log collection
- Azure Monitor Agent (AMA) integration
- Custom Analytics Rules
- KQL-based Threat Hunting
- Security Incident Investigation
- Interactive Microsoft Sentinel Workbook
- Detection Validation through Attack Simulation
- Professional SOC Documentation

---

# 🏗️ Lab Architecture

### Environment Components

- Microsoft Azure
- Microsoft Sentinel
- Log Analytics Workspace
- Azure Monitor Agent (AMA)
- Azure Arc
- Windows 10 Endpoint
- Windows Server 2022
- Active Directory Domain Services (AD DS)
- Sysmon

---

# 🔄 Security Data Flow

```text
Windows Endpoint
        │
Windows Security Logs
Sysmon Logs
        │
        ▼
Azure Monitor Agent (AMA)
        │
        ▼
Log Analytics Workspace
        │
        ▼
Microsoft Sentinel
        │
        ├── Analytics Rules
        ├── Threat Hunting
        ├── Incidents
        └── Workbooks
```

---

# 🛠️ Technology Stack

| Category | Technology |
|----------|------------|
| Cloud Platform | Microsoft Azure |
| SIEM | Microsoft Sentinel |
| Log Management | Azure Log Analytics Workspace |
| Endpoint Monitoring | Azure Monitor Agent (AMA) |
| Identity Management | Active Directory Domain Services |
| Operating Systems | Windows 10, Windows Server 2022 |
| Endpoint Telemetry | Sysmon |
| Query Language | Kusto Query Language (KQL) |
| Virtualization | Oracle VirtualBox |
| Documentation | Markdown, GitHub |

---

# 🛡️ Detection Engineering

This project follows a structured Detection Engineering workflow for designing, validating, and documenting security detections.

### Detection Workflow

1. Identify Threat
2. Collect Security Telemetry
3. Analyze Windows Security & Sysmon Logs
4. Develop KQL Detection Logic
5. Create Microsoft Sentinel Analytics Rules
6. Validate through Attack Simulation
7. Investigate Security Incidents
8. Tune Detections
9. Document Findings

---

# 🚨 Implemented Analytics Rules

| Analytics Rule | Status |
|----------------|:------:|
| Account Lockout Detection | ✅ |
| Domain Controller Successful Logon Monitoring | ✅ |
| Suspicious Process Creation | ✅ |
| Suspicious Network Connection | ✅ |
| DNS Query Monitoring | ✅ |
| File Creation Monitoring | ✅ |
| Image Load Monitoring | ✅ |
| Process Access Monitoring | ✅ |
| Registry Key Creation | ✅ |
| Registry Value Modification | ✅ |

**Total Analytics Rules:** **10**

---

# 🔍 Threat Hunting

The platform includes custom KQL hunting queries for proactive security investigations.

### Hunting Categories

- Failed Authentication Attempts
- Successful Logons
- Account Lockouts
- Active Directory Authentication
- Process Execution Monitoring
- Network Connections
- DNS Activity
- Registry Modifications
- File Creation Events
- Sysmon Events

**Total Hunting Queries:** **10**

---

# 🎯 MITRE ATT&CK Coverage

The implemented detections align with the following ATT&CK tactics:

- Initial Access
- Execution
- Persistence
- Privilege Escalation
- Defense Evasion
- Credential Access
- Discovery

---

# ✅ Detection Validation

Each detection was validated by generating security events and confirming:

- Successful Log Ingestion
- KQL Query Accuracy
- Analytics Rule Execution
- Alert Generation
- Incident Creation
- Investigation Workflow

---

# 📸 Project Screenshots

The repository includes screenshots demonstrating:

## Microsoft Sentinel

- Analytics Rules
- Incidents
- Log Analytics Workspace
- Threat Hunting
- Workbooks

## Active Directory

- Domain Controller
- Active Directory Users and Computers
- Organizational Units (OUs)

## Windows Endpoint

- Azure Monitor Agent
- Sysmon Installation
- Windows Security Events

## Detection Validation

- Alert Generation
- Incident Creation
- KQL Query Results
- Security Event Collection

> Screenshots are available in the `screenshots/` directory.

---

# 📂 Repository Structure

```text
Enterprise-Detection-Threat-Hunting-Platform
│
├── Analytics-rules/
├── architecture/
├── Detections/
├── Hunting-queries/
├── Runbooks/
├── Screenshots/
│
├── README.md
├── CHANGELOG.md
└── CONTRIBUTING.md
```

---

# 💼 Skills Demonstrated

- Microsoft Sentinel Administration
- Detection Engineering
- Threat Hunting
- Incident Investigation
- Active Directory Security Monitoring
- Windows Security Event Analysis
- Sysmon Monitoring
- Kusto Query Language (KQL)
- Azure Monitor Agent (AMA)
- Azure Log Analytics Workspace
- Azure Arc
- SIEM Operations
- Detection Validation
- Technical Documentation

---

# 🚀 Future Enhancements

- Logic Apps & Playbook Automation
- Microsoft Defender Integration
- Detection-as-Code (YAML)
- Multi-stage Attack Correlation
- Expanded MITRE ATT&CK Coverage
- Additional Threat Hunting Scenarios
- Automated Alert Enrichment
- Advanced SOC Dashboards

---

# 👨‍💻 Author

**Danish Mansuri**

**MCA (Cyber Security & Digital Forensics)**  
**Detection Engineering | Threat Hunting | Microsoft Sentinel | SIEM**

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
