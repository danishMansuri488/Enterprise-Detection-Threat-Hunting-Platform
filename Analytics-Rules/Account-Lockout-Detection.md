# Account Lockout Detection

## Purpose
Detect Active Directory account lockout events caused by repeated failed authentication attempts.

## Data Source
- Windows Security Events

## Event ID
- 4740 – A user account was locked out

## MITRE ATT&CK
- T1110 – Brute Force

## Detection Logic
Monitor Windows Security Event ID 4740 to identify user accounts that become locked after multiple failed logon attempts.

## Investigation Steps
- Identify the affected account.
- Review the source computer.
- Check for repeated failed logons (Event ID 4625).
- Determine whether the activity is legitimate or malicious.

## Expected Outcome
Generate a Microsoft Sentinel incident for potential brute-force activity and initiate analyst investigation.
