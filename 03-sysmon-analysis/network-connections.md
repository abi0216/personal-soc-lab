# Sysmon Network Connection Analysis

## Event Type

Sysmon Event ID: 3

Event Name: Network Connection

## Objective

The objective was to understand endpoint network telemetry.

## Information Investigated

- Source process
- Destination IP
- Destination port
- Protocol
- Connection time

## SOC Investigation Questions

- Which process initiated the connection?
- Where is the process located?
- What destination was contacted?
- Which port was used?
- Is the connection expected?

## Investigation Concept

```text
Process Execution
	|
Network Connection
	|
Destination Analysis
	|
SOC Investigation
```

## Key Learning

Network activity becomes much more useful when correlated with process telemetry. The most important question is: which process made the connection?
