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
- subnet ranges must always begin at exact multiple of own subnet size
- ex. `100.0.0.34/29` - `255.255.255.11111000`
	- DOES NOT START AT `100.0.0.34`
	- subnet size is 8
	- possible starting ips (`100.0.0.0`, `100.0.0.8`, `100.0.0.16`, `100.0.0.24`, `100.0.0.32` etc.)