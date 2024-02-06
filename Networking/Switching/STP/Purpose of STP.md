- used to eliminate frame loops
- adds redundancy
- device elected by STP is called the **root bridge**
- prevents looping from
	- broadcast
	- multicast
	- unknown unicast
#### BPDUs
Bridge Protocol Data Units
- contains bridge ID
	- priority value
		- default 32768 (range 0-61440 increments 4096)
		- lower priority is preferable
	- extended system ID
		- decimal value
	- MAC address of switch
		- can be used as a tiebreaker