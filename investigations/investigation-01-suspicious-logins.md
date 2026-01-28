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
- Work in progress — I will run the commands in my Ubuntu VM and update with results + screenshots.

## Conclusion
- Pending results. Will update after reviewing auth.log and syslog.

## Next Steps
- Run log searches in Ubuntu VM
- Add screenshots of outputs
- Summarize normal vs suspicious patterns observed
