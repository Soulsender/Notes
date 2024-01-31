==PERMISSIONS==

(EX.) lrwxrwxrwx
	(l)(rwx)(rwx)rwx
	 1   2    3  4
		
1- first char indicates type of file
	d - directory
	l - symlink
	- - normal file/none

2 - permissions for owner of file

3 - permissions for group associated with file

4 - permissions for all users (world permissions)

rwx - read, write, execute

execute in directory means to execute a command in that directory

==CHMOD==
changes permissions

(EX.) chmod +x
	adds execute permissions to the file

(EX.) chmod g-w
	removes writer permissions for that group

(EX.) chmod a=,u=
	all users have no permissions
	adds read permissions for the user/owner of the file

==CHOWN==
changes ownership

==CHGRP==
changes group ownership
