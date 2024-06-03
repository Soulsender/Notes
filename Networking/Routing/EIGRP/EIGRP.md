### Features
- has authentication
- routing updates are not encrypted
- uses multicast and unicast, NOT broadcast
	- multicast `224.0.0.10` and 
### PDMs
- uses protocol dependant modules (PDMs) for protocols
- maintains EIGRP neighbor and topology tables
- computing metric with DUAL
- filtering and ACLs
### RTP
- transport layer protocol for delivery and reception of EIGRP packets
- not all RTP packets are sent reliably
- `update`, `query`,`reply`
### Packets Types
- hello - used to discover and form adjacencies
	- unreliably sent
	- no ack
- 