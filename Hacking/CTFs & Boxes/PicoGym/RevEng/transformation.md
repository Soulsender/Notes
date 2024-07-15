- file `enc` contains string `灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸彥㜰㍢㐸㙽`
- code snippet is included in challenge
```py
''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])
```
- decoding the string with cyberchef Magic as UTF-16BE gives the flag
- `picoCTF{16_bits_inst34d_of_8_e703b486}`