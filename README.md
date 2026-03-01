## Mini-SOC Lab (Azure + Sentinel)
This project is a hands-on Mini Security Operations Centre built in Microsoft Azure using Microsoft Sentinel.
The goal was to simulate a real-world SOC environment by ingesting endpoint telemetry, validating logs, and preparing for detection engineering and threat hunting.
Built as part of my cybersecurity portfolio to demonstrate practical SIEM and cloud security skills.


## Architecture
Windows 11 VM (Sysmon)
→ Azure Monitor Agent (AMA)
→ Data Collection Rule (DCR)
→ Log Analytics Workspace (LAW)
→ Microsoft Sentinel (Defender XDR)


## What I Implemented
- Azure resource group and cost-controlled environment
- Windows 11 VM with security configurations (Secure Boot, vTPM)
- Sysmon deployment using SwiftOnSecurity config
- Azure Monitor Agent + Data Collection Rules
- Log ingestion into Log Analytics Workspace
- Microsoft Sentinel integration for querying and monitoring
- KQL queries to validate telemetry ingestion



### Skills
- SIEM: Microsoft Sentinel
- Log Management: Azure Log Analytics
- Endpoint Telemetry: Sysmon
- Cloud Security: Azure infrastructure
- Detection Engineering (foundations)
- KQL (Kusto Query Language)
- Security Monitoring Pipeline Design
