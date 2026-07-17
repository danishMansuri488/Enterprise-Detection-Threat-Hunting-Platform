# Architecture

## Overview

This project simulates an enterprise Security Operations Center (SOC) using Microsoft Sentinel to collect, analyze, detect, and investigate security events generated from Windows endpoints and an Active Directory environment.

## Components

- Microsoft Azure
- Microsoft Sentinel
- Log Analytics Workspace
- Azure Monitor Agent (AMA)
- Azure Arc
- Windows Server 2022
- Active Directory Domain Services (AD DS)
- Windows 10 Endpoint
- Sysmon

## Data Flow

Windows Endpoint & Active Directory  
↓  
Azure Monitor Agent (AMA)  
↓  
Log Analytics Workspace  
↓  
Microsoft Sentinel  
↓  
Analytics Rules • Threat Hunting • Incidents • Workbooks
