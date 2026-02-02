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

## Commands Used
```bash
sudo grep "sudo" /var/log/auth.log
sudo grep "COMMAND=" /var/log/auth.log

```
## Findings
- Reviewed sudo-related events in auth.log.
- Identified multiple sudo executions by the local user `kimberly`.
- Commands executed included log review and system-related utilities (grep, tail, update-notifier).
- All sudo activity appeared user-initiated and consistent with normal administrative tasks.
- No unauthorized users or unusual command patterns were observed.

## Conclusion
Based on the review of sudo activity, no suspicious or unauthorized privileged command execution was identified. Observed sudo usage aligns with expected administrative behavior during system analysis. No escalation is required at this time.

## Next Steps
- Continue monitoring sudo usage for anomalies
- Review logs periodically for unauthorized privilege escalation

## Evidence
![Sudo activity](../screenshots/sudo-activity.png)
![Sudo commands](../screenshots/sudo-commands.png)
