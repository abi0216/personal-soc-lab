# Wazuh Windows Agent Monitoring

## Objective

The objective of this lab was to connect a Windows endpoint to the Wazuh server and monitor endpoint telemetry.

## Components

- Wazuh Server
- Wazuh Windows Agent
- Windows Event Logs
- Sysmon

## Result

The Windows agent successfully communicated with the Wazuh server. Windows telemetry was received and became available for investigation.

## Important Learning

Not every event collected by Wazuh automatically becomes an alert. An event may exist in archives, logs, or indexed data without generating a high-priority alert.

```text
Telemetry != Automatically Malicious

Telemetry
	|
Detection Rule
	|
Alert
	|
SOC Investigation
```

SOC analysts must understand the difference between raw events, detection rules, alerts, false positives, and legitimate activity.

## Screenshots

Add Wazuh agent connected, agent details, and Windows telemetry visible in Wazuh. Do not put all Sysmon investigations here.
