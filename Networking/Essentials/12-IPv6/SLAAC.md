#ipv6 
- allows devices to configure GUA without DHCPv6
- devices obtain info for GUA from ICMPv6 RA messages of the router
- prefixes are provided by the RA and the device uses either EUI-64 (mac address + fffe) or random gen method to create interface ID