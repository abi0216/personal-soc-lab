# Sysmon Process Creation Analysis

## Event Type

Sysmon Event ID: 1

Event Name: Process Creation

## Objective

The objective was to understand how Sysmon records process execution and parent-child relationships.

## Example Activity

PowerShell was launched from Windows Explorer.

```text
Explorer.exe
	|
PowerShell.exe
```

## Important Fields Investigated

- Image
- ParentImage
- User
- ProcessId
- CommandLine
- Hashes

## SOC Investigation Process

1. Identify the process.
2. Identify the parent process.
3. Check the process location.
4. Check the user account.
5. Review the command line.
6. Determine whether the behavior is expected.

## Important Learning

A process is not malicious simply because it is PowerShell. SOC analysis requires context. The same process may be legitimate, unusual, suspicious, or malicious depending on its execution context.

## Screenshots

Add screenshots showing Sysmon Event ID 1, the parent-child relationship, and process fields.
