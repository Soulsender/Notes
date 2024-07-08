#exam
### OSPF
- LSUs contain different link-state advertisements
- hello > DBD > LSR > LSU > LSA
- down > init >two-way > exstart > exchange > loading > full
- lower priority, highest RID
### ACLs
- routers can have 4 acls on one interface
	- in/out IPv4
	- in/out IPv6
### NAT
- NAT64 used to provide access for IPv4 and IPv6 only networks
### WAN
- single-homed
	- connects to ISP with one link
- dual-homed
	- connects to ISP with two links
- multihomed
	- connects to two different ISPs; one link each
- dual-multihomed
	- connects to two different ISPs; two links each
- ISPs use PPP
	- authentication
	- assign public IPv4 addr\
	- link-quality management features
	- ethernet does not support PPP
### VPN
- GRE; tunnel only, no encryption
- site-to-site; between routers
- remote access; client has VPN client software
- HTTPS is clientless VPN
### QoS
- FIFO (first in first out)
	- is default
- WFQ (weighted fair queuing)
	- classifies traffic by priority
	- uses packet headers src/dst IPs, MACs, port numbers, protocol, & ToS (in IP header)
	- cannot be used with tunneling/encryption
- CBWFQ (class based weighted fair queuing)
	- extends WFQ with user classes
	- can be used with tunneling/encryption
- LLQ (low latency queuing)
	- sends delay sensitive packets first
	- used with CBWFQ
- shaping doesn't drop packets, it sends at a different time
- policing drops packets when it is overwhelmed
### Network Management
- syslog (DINWECAE) 8 total
	- 0 emergency
	- 7 debug
- troubleshooting
	- define problem > gather info > analyze info > eliminate causes > propose hypothesis > test > solve