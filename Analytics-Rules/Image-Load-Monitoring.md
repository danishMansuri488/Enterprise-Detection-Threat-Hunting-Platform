# Image Load Monitoring

## Purpose
Detect suspicious Dynamic Link Library (DLL) or executable image loading that may indicate malicious code execution.

## Data Source
- Sysmon Operational Logs

## Event ID
- 7 (Image Loaded)

## MITRE ATT&CK
- T1574 – Hijack Execution Flow

## Detection Logic
Monitor Sysmon Image Load events to identify unusual or unauthorized DLL and executable image loading on monitored systems.

## Investigation Steps
- Review the loaded image name.
- Verify the loading process.
- Check the image path and digital signature.
- Determine whether the activity is legitimate or suspicious.

## Expected Outcome
Generate a Microsoft Sentinel incident for suspicious image loading requiring analyst investigation.
