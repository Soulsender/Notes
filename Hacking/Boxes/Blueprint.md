### Enumeration
- PHP application `oscommerce-2.3.4`
	- https://www.exploit-db.com/exploits/44374
### Metasploit
- `exploit(multi/http/oscommerce_installer_unauth_code_exec`
- gain shell as php app user
- create meterpreter revshell executable with msfvenom
- run metasploit listener `windows/meterpreter/reverse_tcp`
- gain shell and hashdump
- password for `Lab:googleplus`