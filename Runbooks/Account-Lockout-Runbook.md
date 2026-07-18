# Account Lockout Investigation Runbook

## Purpose

Investigate account lockout events to determine whether they are caused by brute-force attacks, password spraying, stale credentials, or legitimate user activity.

## Detection Source

- Microsoft Sentinel
- Windows Security Event ID: 4740

## Investigation Steps

1. Review the generated Microsoft Sentinel alert.
2. Identify the locked user account.
3. Determine which computer initiated the lockout.
4. Review recent failed logon events (Event ID 4625).
5. Check for successful logons before the lockout.
6. Verify whether the activity is malicious or expected.

## Evidence Collection

- SecurityEvent (4740)
- SecurityEvent (4625)
- SecurityEvent (4624)
- User account details
- Source computer information

## Containment

- Disable the account if compromise is suspected.
- Block malicious source systems if necessary.
- Notify the affected user.

## Recovery

- Reset the user's password.
- Unlock the account.
- Confirm successful authentication after recovery.

## Lessons Learned

Review authentication policies and detection rules to reduce future account lockouts.
