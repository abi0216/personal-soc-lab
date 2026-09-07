# File Integrity and Registry Monitoring

## Objective

The objective was to understand how Wazuh detects changes to monitored files and registry entries.

## Activity Observed

A registry integrity event was observed involving a Windows service-related registry location. The event indicated a registry key entry change or deletion.

## Detection Context

The event was associated with registry monitoring and integrity detection. MITRE ATT&CK mappings were provided by the monitoring platform.

## Important Learning

A security alert does not automatically mean an attack occurred. Registry and system configuration changes can be caused by legitimate software, Windows updates, administrative activity, service changes, or malicious activity.

## SOC Investigation Questions

- Which process caused the change?
- Which user performed the activity?
- Was the change expected?
- Did other suspicious events occur nearby?
- Is the affected registry location security-sensitive?

## Screenshots
<img width="1897" height="951" alt="image" src="https://github.com/user-attachments/assets/c21ded3f-d03d-4634-9fa9-a91cbd98593e" />

Overview of the threat hunting

<img width="1919" height="969" alt="image" src="https://github.com/user-attachments/assets/a3ca219e-d970-4fcc-ab62-988cd50cac0b" />

Inspection of the particular process

