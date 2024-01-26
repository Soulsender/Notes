- 22 - ssh
	- login `jeanpaul/I_love_java`
	- sudo -l
		- can use zip as sudo
	- [gtfobins](https://gtfobins.github.io) gives command for zip root shell

- 2049 - nfs fileshare
	- encrypted zip file
	- bruteforce with `fcrackzip -v -u -D -p ~/wordlists/rockyou.txt save.zip`
		- id_rsa for ssh with -i
		- todo.txt with things about loving java
			- signed by jp

- 8080 - php default page
	- Linux dev 4.19.0-16-amd64 #1 SMP Debian 4.19.181-1 x86_64

- 80 - Apache httpd 2.4.38 
	- /app/config has SQL login in config.yml
		- login `bolt/I_love_java` -> ssh login `jeanpaul/I_love_java`
	- /dev has boltwire login page
		- messing with path can give user on server ``
	- subdirectories -> [Feroxbuster](./Feroxbuster)
	- Faulty Bolt installation?
	- ![[Pasted image 20221029221605.png]]