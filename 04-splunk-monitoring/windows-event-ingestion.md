# Windows Event Log Ingestion

## Objective

The objective was to verify that Windows Event Logs were successfully ingested into Splunk.

## Verification

A broad Splunk search was performed to verify incoming events. Windows Security events were successfully observed.

Example source information included:

- Host
- Source
- Sourcetype
- EventCode
- ComputerName

## Example Data Source

```text
Source:
WinEventLog:Security

Sourcetype:
WinEventLog:Security
```

## Result

Windows event ingestion into Splunk was successfully verified.

```text
Windows
	|
Splunk Universal Forwarder
	|
Splunk Enterprise
	|
SOC Investigation
```

## Important Learning

Before investigating attacks, a SOC analyst must first confirm that telemetry is being collected correctly.

> No telemetry -> No detection -> No investigation
