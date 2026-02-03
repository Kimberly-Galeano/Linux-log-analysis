# Investigation 03 – User Account & Login Review

## Objective
Review local user accounts and login activity to identify any unauthorized or unusual user behavior.

## Environment
- Ubuntu Linux (VirtualBox VM)

## Data Reviewed
- /etc/passwd
- /etc/shadow (awareness only)
- Login history (who, last)

## Investigation Steps
1. Reviewed local user accounts
2. Identified users with login shells
3. Checked recent login activity
4. Evaluated whether accounts and logins appeared expected

## Commands Planned
```bash
cat /etc/passwd
grep "/bin/bash" /etc/passwd
who
last

## Findings
- Pending analysis. Results will be documented after reviewing local user accounts and login activity.
- Findings will focus on identifying authorized users, login-capable accounts, and recent login behavior.

## Conclusion
- Pending review. A conclusion will be documented after evaluating user accounts and login history.

## Next Steps
- Run user and login-related commands in the Ubuntu VM
- Capture screenshots of relevant command output
- Determine whether any unauthorized or suspicious user accounts or login activity exist
