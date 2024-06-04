#routing #eigrp
### Features
- has authentication
- routing updates are not encrypted
- uses multicast and unicast, NOT broadcast
	- multicast `224.0.0.10` and `ff02::a`
### PDMs
- uses protocol dependent modules (PDMs) for protocols
- maintains EIGRP neighbor and topology tables
- computing metric with DUAL
- filtering and ACLs
- allows support for different layer 3 protocols
### RTP
- transport layer protocol for delivery and reception of EIGRP packets
- not all RTP packets are sent reliably
- `update`, `query`,`reply`
### Packets Types
- hello 
	- used to discover and form adjacencies
	- unreliably sent, no ack
- update
	- sent initially for topology info
	- reliable, needs ack
	- only contain relevant routing info
	- unicast
- query, reply
	- used by DUAL when searching for network
	- reliable, needs ack
	- queries are multicast/unicast
	- reply are unicast
### Messages
- EIGRP frame destination multicast `01:00:5e:00:00:0a`
- IP header `224.0.0.10:88`
### Autonomous System (AS)
- collection of networks under authority
- AS numbers used to exchange routes
- managed by IANA
