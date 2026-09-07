# Sysmon File Creation Analysis

## Event Type

Sysmon Event ID: 11

Event Name: File Creation

## Objective

The objective was to observe how a process creates a file and how Sysmon records the activity.

## Example Activity

A process created a file inside the Downloads directory.

```text
Process
	|
Creates File
	|
Sysmon Event
```

## Important Fields

- Image
- TargetFilename
- User
- Process information
- Time of activity

## SOC Investigation Questions

- Which process created the file?
- Where was the file created?
- Is the location unusual?
- Is the file extension suspicious?
- Is the parent process expected?

## Key Learning

File creation telemetry can help identify malware downloads, dropped payloads, script-generated files, and suspicious executable creation. File creation must still be investigated with context.
