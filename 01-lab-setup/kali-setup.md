# Kali Linux Lab Setup

## Purpose

Kali Linux is used as the security testing machine in my authorized SOC lab environment.

The machine generates controlled security activities that can later be observed and investigated from the defender perspective.

## Role in the Lab

Kali Linux is used for:

- Network connectivity testing
- Network reconnaissance
- Service discovery
- Controlled authentication testing
- Authorized attack simulation

## Communication

Kali Linux can communicate with the authorized Windows machine used in this lab. This connectivity is required to simulate realistic network activity.

## SOC Learning Perspective

```text
Activity generated on Kali
	|
Activity received by Windows
	|
Windows generates telemetry
	|
Logs forwarded to SIEM
	|
SOC analyst investigates evidence
```

## Future Controlled Activities

- Network reconnaissance
- Service discovery
- Authentication monitoring
- Controlled failed login scenarios

All activities will be performed only against authorized lab systems.

## Screenshots

Add Kali Linux desktop or terminal, network configuration, and connectivity test screenshots.

Do not put every command used, attack tutorials, or results from future detection labs here.
