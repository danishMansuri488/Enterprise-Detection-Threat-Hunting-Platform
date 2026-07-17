# Domain Controller Successful Logon Monitoring

## Purpose
Monitor successful logon events on the Domain Controller to detect account activity and identify unusual authentication patterns.

## Data Source
- Windows Security Events

## Event ID
- 4624 (An account was successfully logged on)

## MITRE ATT&CK
- T1078 – Valid Accounts

## Detection Logic
Monitor successful logon events on the Domain Controller to identify authentication activity performed by users and administrators.

## Investigation Steps
- Verify the user account.
- Review the source computer.
- Confirm the logon time and logon type.
- Identify any unusual or unauthorized access.

## Expected Outcome
Generate a Microsoft Sentinel incident for suspicious or unexpected successful logon activity requiring analyst review.
