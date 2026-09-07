# Network Architecture

## Objective

The objective of this lab is to simulate controlled cybersecurity activities from Kali Linux against an authorized Windows machine and investigate the generated telemetry using security monitoring tools.

## Lab Machines

### Kali Linux

Role: Lab attacker / security testing machine

Purpose:

- Network reconnaissance
- Controlled security testing
- Service discovery
- Attack simulation in an authorized environment

Network IP:

[Add your lab IP here if you want to document it]

### Windows Machine

Role: Monitored target machine

Purpose:

- Receive controlled lab activity
- Generate Windows Event Logs
- Generate Sysmon telemetry
- Forward telemetry to Splunk

Important:

This machine is my own authorized Windows system used only for controlled lab testing.

## Network Connectivity

The Kali Linux machine and Windows machine can communicate successfully.

Example validation:

```text
Kali Linux
	|
Ping
	|
Windows Machine
	|
Reply Received
```

This confirms that the lab machines can communicate and controlled network activities can be performed.

## Security Monitoring Architecture

```text
Kali Linux
	|
Controlled Security Activity
	|
Windows Machine
	|
Windows Event Logs + Sysmon
	|
Splunk Universal Forwarder
	|
Splunk Enterprise
	|
SOC Investigation
```

## Key Learning

This architecture allows me to understand the complete SOC investigation lifecycle:

Attacker Activity -> Endpoint Telemetry -> Log Collection -> SIEM Investigation

## Screenshots

Add screenshots showing:

- Kali Linux
- Windows connectivity
- Successful ping between lab machines
- Overall lab architecture

Do not put Wazuh alert details, Sysmon Event ID analysis, SPL queries, or incident reports here. Those belong in later folders.
