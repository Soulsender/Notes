*Bridge Protocol Data Units*
- contains bridge ID
	- priority value
		- default 32768 + vlan number (range 0-61440 increments 4096)
		- lower priority is preferable
	- MAC address of switch
		- can be used as a tiebreaker