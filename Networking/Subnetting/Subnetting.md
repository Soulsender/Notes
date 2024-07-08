### Subnets based on hosts
- add 2 to number of hosts
- ex. 5 hosts
	- smallest power of 2 that is >= 7
	- 2^3 = 8
### Find hosts on subnet
- subtract octet from 256 then multiply together
- ex. `255.255.255.248`
	- 1 * 1 * 1 * 8 = 8 hosts
### Finding subnet size
- you cannot start at any ip
- ex. `100.0.0.34/29`
	- 