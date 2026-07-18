# Authentication Monitoring Metrics

## Purpose

Track authentication activity to identify abnormal login behavior and evaluate the effectiveness of authentication monitoring.

## Metrics

| Metric | Description |
|----------|-------------|
| Successful Logons | Total successful user authentication events (Event ID 4624). |
| Failed Logons | Total failed authentication attempts (Event ID 4625). |
| Account Lockouts | Number of account lockout events (Event ID 4740). |
| Privileged Logons | Number of privileged account logon events. |

## Data Source

- Microsoft Sentinel
- Windows Security Events

## Objective

These metrics help identify authentication trends, detect brute-force attempts, and monitor user account activity across the environment.
