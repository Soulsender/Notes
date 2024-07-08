#dhcp 
- generated GUA either randomly or with EUI64 (MAC address)
- DAD process is used to verify address is not already used
- finds default gateway via router advertisements sent from link router
### Process
1. host generates address
2. host sends ICMPv6 **neighbour solicitation** w/ its own IP as target
3. if no other devices respond with **neighbour advertisement** then address is unique