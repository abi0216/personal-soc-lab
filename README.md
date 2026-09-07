# Personal SOC Lab

A hands-on cybersecurity lab focused on learning Security Operations Center (SOC) investigation, Windows telemetry analysis, threat detection, and incident investigation.

## 🎯 Objective

The goal of this lab is to develop practical SOC Analyst skills by performing controlled security activities in an authorized lab environment and investigating the generated telemetry.

The learning workflow is:

Simulated Activity
        ↓
Windows Machine
        ↓
Windows Event Logs + Sysmon
        ↓
Splunk / Wazuh
        ↓
SOC Investigation
        ↓
Detection & Analysis
        ↓
MITRE ATT&CK Mapping
        ↓
Documentation

                 ┌─────────────────┐
                 │   Kali Linux    │
                 │  Lab Machine    │
                 └────────┬────────┘
                          │
                 Controlled Activity
                          │
                          ▼
                 ┌─────────────────┐
                 │ Windows Machine │
                 │ Victim / Target │
                 └────────┬────────┘
                          │
              Windows Logs + Sysmon
                          │
                          ▼
                 ┌─────────────────┐
                 │ Splunk Forwarder│
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Splunk Enterprise│
                 │ SOC Investigation│
                 └─────────────────┘
                 
🛠️ Technologies Used

Kali Linux
Windows
Sysmon
Wazuh
Splunk Enterprise
Splunk Universal Forwarder
PowerShell
Windows Event Logs
VirtualBox
MITRE ATT&CK Framework

🔍 Hands-On Learning Areas

Windows Event Log Analysis
Sysmon Telemetry Analysis
Process Creation Investigation
Parent-Child Process Analysis
File Creation Monitoring
DNS Investigation
Network Connection Analysis
File Integrity Monitoring
Registry Monitoring
Authentication Monitoring
Brute-Force Detection
Suspicious PowerShell Detection
SPL Detection Engineering
Incident Investigation
MITRE ATT&CK Mapping

## Lab Workflow

```text
Controlled Activity -> Endpoint Telemetry -> Log Collection -> SIEM Investigation
```

## Documentation Sections

- [Lab setup](01-lab-setup/)
- [Wazuh monitoring](02-wazuh-monitoring/)
- [Sysmon analysis](03-sysmon-analysis/)
- [Splunk monitoring](04-splunk-monitoring/)
- [SOC detection labs](05-soc-detection-labs/)
- [Incident investigations](06-incident-investigations/)

Screenshots are stored under `screenshots/`. All activities are performed only against authorized lab systems.
