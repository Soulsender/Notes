#ospf 
https://www.youtube.com/watch?v=kfvJ8QVJscc
- routers send out LSAs (link-state advertisement)
- all LSAs are kept a database (LSDB)
	- all routers should end up having the same information in their LSDBs
#### Steps
- becoming neighbors
	- two routers running OSPF agree on the same link to form neighbor relationship
- exchanging LSDB info
- choosing best routes
	- routers choose best route based on learned LSDB info
	- SPF calculation
#### Prerequisites
- routers must choose router ID (RID)
	- formats in IPv4 address
	- if automatic
		- router will choose highest "up" status loopback interface
		- router will choose highest "up" non-loopback interface
#### Packets
- hello
	- RID
	- already known neighbors
	- also work as uptime messages 
#### DR & BDR
- elected based on highest ESPF priority
	- set to 1 by default (can be changed)