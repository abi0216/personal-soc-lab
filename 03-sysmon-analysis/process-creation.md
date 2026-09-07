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

<img width="1262" height="978" alt="image" src="https://github.com/user-attachments/assets/c2b54a62-6a6b-48d5-9dd2-680a2aa7d659" />

