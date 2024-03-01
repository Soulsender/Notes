### Logging
> Don't Idle Near West End Chicago At Evening
- 8 predefined priorities
	- emerg
	- alert
	- crit
	- err
	- warning
	- notice
	- info
	- debug
- `/etc/rsyslog.conf` and `/etc/rsyslog.d/`
- `rsyslogd` daemon
### Find
- `-type l` for symbolic links
- `-links +1` for hard links
- `-iname` like `-name` but case insensitive
- locate will match files with filename contains specified text
- find will match EXACT NAMES (no file extension unless specified)
### Scripts
- `echo -n` removes the newline and any space at the end
- `elif` NOT `elseif` or `else if`
### Scheduling
- `atrm 2` to remove the second job
- `atq` to list all jobs
- `0 0 13 * fri` every friday OR 13th of every month