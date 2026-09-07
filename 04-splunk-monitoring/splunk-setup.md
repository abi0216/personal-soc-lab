# Splunk Enterprise SOC Lab Setup

## Objective

The objective was to configure Splunk Enterprise for Windows security monitoring and investigation.

## Architecture

```text
Windows Machine
	|
Splunk Universal Forwarder
	|
Splunk Enterprise
	|
Search and Investigation
```

## Data Sources

Windows Event Logs were configured for collection:

- Security
- System
- Application
- Setup

## Result

Windows events were successfully received by Splunk. This confirmed that the data pipeline was working.

## Key Learning

A SIEM is useful only when logs are collected, data is searchable, important fields are extracted, and analysts can investigate the events.
