### Enumeration
- HTTP (80), SMTP (25), POP3 (55007)
### HTTP (80)
- Encoded password hidden in `/terminal.js`
	- HTML character codes
	- `&#73;&#110;&#118;&#105;&#110;&#99;&#105;&#98;&#108;&#101;&#72;&#97;&#99;&#107;&#51;&#114;`
- `/sev-home` login `boris:InvincibleHack3r`
- user `natalya` in HTML source code
### POP3 (55007)
- bruteforce for `boris:secret1!`
- bruteforce for `natalya:bird`
- potential user `alec`
### severnaya-station.com/gnocertdir
- user creds `xenia:RCP90rulez!`
- another user called `doak`
- user cred `dr_doak:4England!`
- `s3cret.txt` in private files
- leads to `/dir007key/for-007.jpg` on webserver
- image contains base64 encoded password `admin:xWinter1995x!`
- spellcheck plugin:
	- change path to reverse shell
	- change spell check to PSpellShell
	- enable spellcheck in a new blog entry so the server tries to read that path
### Kernel exploit 
- kernel version 3.13.0-32-generic
- vulnerable to [overlayfs](https://www.exploit-db.com/exploits/37292) kernel exploit
- exploit has to be compiled with clang not gcc (`sed -i "s/gcc/cc/g" overlayfs.c && cc overlayfs.c -o overlayfs`)
- flag is at `/root/.flag.txt`