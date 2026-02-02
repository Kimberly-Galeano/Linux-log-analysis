# Investigation 02 – Sudo (Privilege) Activity Review

## Objective
Review sudo usage to identify any unusual or unauthorized privileged command execution.

## Environment
- Ubuntu Linux (VirtualBox VM)

## Data Reviewed
- /var/log/auth.log

## Investigation Steps
1. Reviewed auth.log for sudo-related events
2. Identified which users executed sudo commands
3. Reviewed the commands that were run with elevated privileges
4. Evaluated whether the activity appeared normal or suspicious

## Commands Planned
```bash
sudo grep "sudo" /var/log/auth.log
sudo grep "COMMAND=" /var/log/auth.log

```
## Findings
- Work in progress. Results will be added after reviewing sudo-related activity.

## Conclusion
- Pending analysis. Will update after reviewing sudo command usage.

## Next Steps
- Run sudo-related log searches
- Capture screenshots of relevant output
- Determine whether sudo usage appears expected or suspicious
