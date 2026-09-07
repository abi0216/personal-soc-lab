# Sysmon DNS Monitoring

## Event Type

Sysmon Event ID: 22

Event Name: DNS Query

## Objective

The objective was to understand how DNS queries can be used during SOC investigations.

## Information Available

- Query name
- Source process
- Process information
- Query time

## SOC Investigation Value

DNS activity can help identify suspicious domains, malware communication, command-and-control infrastructure, and unusual external destinations.

## Investigation Workflow

```text
Suspicious Process
	|
DNS Query
	|
Domain Investigation
	|
Correlation with Other Events
```

## Important Learning

A DNS query alone does not prove malicious activity. The query should be correlated with process creation, network connections, file activity, and threat intelligence.
