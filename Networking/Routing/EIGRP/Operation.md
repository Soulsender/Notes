#eigrp 
### Example
- R1 joins routing domain
- sends EIGRP hello to all EIGRP ports
- R2 receives hello, adds R1 to neighbor table
- R2 sends update packet with all routes it knows
- R2 sends hello to R1
- R1 updates neighbor table with R2
- R1 sends ack
- R1 sends update packet with all known routes (except R2's known) to R2
- R2 sends ack
- R1 and R2 use DUAL to calculate best routes
### Metrics
- bandwidth
- delay
- reliability (optional)
- load (optional)
### DUAL (diffusing update algorithm)
- successor
	- neighboring router for packet forwarding
	- least cost
- feasible successors (FS)
	- backup paths
- reported distance (RD)
	- advertised distance
- feasible distance (FD)
	- actual metric of route
- states
	- passive - available for use
	- active - route is being recomputed by DUAL
