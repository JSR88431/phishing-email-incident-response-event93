# Incident Report

## Summary
A phishing email containing a malicious Excel macro attachment was delivered to a user. Execution of the attachment resulted in system compromise.

## Timeline
- Email received
- Attachment opened
- Macro executed
- regsvr32 process spawned
- External connections initiated

## Impact
- Endpoint compromised
- Potential data exfiltration risk

## Response Actions
- Isolated affected host
- Blocked malicious domains
- Removed email from inbox

## Lessons Learned
- Macro-enabled attachments remain a major threat
- Endpoint monitoring is critical
