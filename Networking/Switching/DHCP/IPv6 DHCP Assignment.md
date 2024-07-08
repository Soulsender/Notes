#dhcp 
#### Stateful DHCP
- uses DHCP server fully to get IPv6 address
#### Stateless DHCP
- uses a combination of SLAAC and a DHCP server to make its own address based off info from the DHCP server
#### SLAAC
- device makes address all on its own
## Message Flags
- `A=1 O=0 M=0` - SLAAC
- `A=1 O=1 M=0` - Stateless DHCP/SLAAC
- `A=0 O=0 M=1` - Stateful DHCP only