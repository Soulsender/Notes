#ospf 
- link state routing protocol
- alternative for RIP
#### Packets
- hello
	- only sent to neighbours
	- every few minutes (keep alive)
	- sent to multicast 224.0.0.5
- database description
	- tells neighbour about known neighbours
- link-state request
	- asking to know more about networks it can't reach
- link-state update
	- sending info about networks a neighbour can't reach
- link-state acknowledgement
#### Data Structures
- adjacency database
	- creates neighbour table
		- lists neighbour routers for routers with bidirectional comms
		- unique for each router
		- `show ip ospf neighbor`
- link-state database (LSDB)
	- creates topology table
		- info about other routers
		- represents network topology
		- all routers have identical LSDB
		- `show ip ospf database`
- forwarding database
	- creates routing table
		- list of routes generated when algorithm is run on LSDB
		- routing table on each router is unique
		- `show ip route`
#### Algorithms
- uses SPF algorithm
- creates tree by putting each router at root of tree, then calculates shortest path to each node