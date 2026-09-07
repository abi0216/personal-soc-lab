# SPL Queries

## Purpose

This file contains SPL queries used during SOC lab investigations.

## View All Events

### Query

```spl
index=*
```

### Purpose

Used to verify that events are being received by Splunk.

### What to Look For

- Event volume
- Hosts
- Sources
- Sourcetypes

## Security Events

### Query

```spl
source="WinEventLog:Security"
```

### Purpose

Used to focus on Windows Security Event Logs.

## Notes

Each query added to this document should include the query, purpose, expected output, and investigation value. Only add queries that are actually tested and understood.
