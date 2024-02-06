- used to eliminate frame loops
- adds redundancy
- device elected by STP is called the **root bridge**
- prevents looping from
	- broadcast
	- multicast
	- unknown unicast
#### Root Ports
- best route to the root bridge
	- based on port cost
	- root cost -> my BID -> root BID
![[attachments/image/Purpose of STP-1707255207413.jpeg]]
#### Timers
- **hello timer** 2 secs
- **forward delay timer** 15 secs
- **max age timer** 20 secs
