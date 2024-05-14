NMAP

255.255.255.0 - /24
255.255.0.0 - /16
255.0.0.0 - /8

-sN 	- ping
-T4		- 4/5 power scan
-A		- everything
-p- 	- all ports
-sU 	- UDP (takes forever)
-oN 	- output file

nmap -sC -sV -oN nmap-initial.log
nmap -A -T4 -p- -oN nmap-deep.log
