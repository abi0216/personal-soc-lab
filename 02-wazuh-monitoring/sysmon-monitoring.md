# Sysmon Monitoring with Wazuh

## Objective

The objective was to observe Sysmon endpoint telemetry through Wazuh.

## Sysmon Telemetry Observed

- Process creation
- File creation
- DNS queries
- Network activity

## Example Investigation Concept

```text
Process executes
	|
Sysmon records activity
	|
Wazuh receives telemetry
	|
SOC analyst investigates process context
```

## Important Learning

Sysmon provides detailed endpoint telemetry that can help investigators understand which process executed, which parent process started it, which user executed it, which files were created, and which network destinations were contacted.

An event should not automatically be considered malicious. Investigate process path, parent process, user, command line, destination, and time.
