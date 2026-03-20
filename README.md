# Phishing Email Investigation (Event ID 93)

## Overview
This project documents a phishing email investigation conducted in the LetsDefend SOC environment. The alert involved a malicious Excel 4.0 macro attachment used to compromise a host system.

## Alert Details
- Event ID: 93
- Alert Name: Phishing Mail Detected – Excel 4.0 Macros
- Severity: High

## Scenario
A suspicious email containing a macro-enabled attachment was reported. The investigation focused on identifying whether the email was malicious and determining the extent of impact.

## Investigation Steps
1. Reviewed alert in SOC dashboard
2. Analyzed sender and email metadata
3. Extracted and analyzed attachment
4. Checked file hash using VirusTotal
5. Investigated endpoint activity
6. Reviewed network connections

## Key Findings
- Malicious Excel macro executed on host
- Excel spawned regsvr32 process
- DLL files registered on system
- Outbound connections to suspicious domains

## Indicators of Compromise
See: ioc/indicators.md

## MITRE ATT&CK Mapping
- T1566 – Phishing
- T1204 – User Execution
- T1071 – Command and Control
- T1547 – Persistence

## Conclusion
The alert was confirmed as a true positive phishing attack resulting in system compromise.

## Screenshots
See the `screenshots/` folder for full investigation evidence.
