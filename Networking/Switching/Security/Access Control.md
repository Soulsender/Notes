### 802.1x
- port based access control; workstations are authenticated with a server
- client (supplicant)
- switch (authenticator)
- auth server
### Layer 2 Attack Mitigation
- port security (MAC whitelisting)
	- manual - statically configured by admin
	- dynamic - current source MAC is used; does not persist past reload
	- dynamic sticky - current MAC is used; stuck in configuration
- DHCP snooping
- dynamic ARP inspection
- IP source guard