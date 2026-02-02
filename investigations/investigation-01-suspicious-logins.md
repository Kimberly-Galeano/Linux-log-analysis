# Investigation 01 – Suspicious Login Activity

## Objective
Review Linux authentication logs to identify any unusual or suspicious login activity.

## Environment
- Ubuntu Linux (VirtualBox VM)

## Data Reviewed
- /var/log/auth.log
- /var/log/syslog

## Investigation Steps
1. Reviewed authentication logs to understand normal login behavior
2. Searched for failed login attempts
3. Looked for repeated login attempts from the same source
4. Noted timestamps and usernames involved

## Commands Used
```bash
cat /var/log/auth.log
grep "Failed password" /var/log/auth.log
grep "Accepted password" /var/log/auth.log
```

## Findings
- A small number of failed password attempts were observed.
- Failed login activity appeared limited and not repetitive.
- Successful login activity matched expected user behavior.
- No evidence of brute-force or unauthorized access was identified.

## Conclusion
Based on the review of authentication logs, no suspicious login activity was identified. 
Observed failed login attempts were minimal and consistent with normal user behavior. 
No further investigation is required at this time.

## Next Steps
- Run log searches in Ubuntu VM
- Add screenshots of outputs
- Summarize normal vs suspicious patterns observed

## Evidence
![Auth log recent activity](../screenshots/authlog-tail.png)
![Failed password count](../screenshots/failed-password-count.png)

