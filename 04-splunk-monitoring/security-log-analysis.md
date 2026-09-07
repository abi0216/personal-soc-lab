# Windows Security Log Analysis

## Objective

The objective was to explore Windows Security logs in Splunk and understand the available investigation fields.

## Example Fields Observed

- Account_Name
- Account_Domain
- ComputerName
- EventCode
- LogName
- Logon_ID
- Process_Name
- Security_ID

## SOC Investigation Value

Security logs can provide evidence related to authentication, account activity, logon events, and security-related actions.

## Investigation Approach

1. Identify the EventCode.
2. Identify the user account.
3. Identify the system.
4. Review the time.
5. Correlate with nearby events.

## Key Learning

A single event provides limited context. SOC investigations require correlation between multiple events.
