#acls 
### 802.1x
- port based access control; workstations are authenticated with a server
- client (supplicant)
- switch (authenticator)
- auth server
### Layer 2 Attack Mitigation
- port security (MAC whitelisting)
- DHCP snooping
- dynamic ARP inspection
- IP source guard
- BPDU Guard
	- disables ports that receive BPDU on access port
### Port Security
- address modes
	- manual - statically configured by admin
	- dynamic - current source MAC is used; does not persist past reload
	- dynamic sticky - current MAC is used; stuck in configuration
- violation modes
	- shutdown - port does into disabled; must be reenabled by admin
	- restrict - port drops packets from unknown source MACs until drops below max value; sends syslog message
	- protect - same as restrict; no syslog