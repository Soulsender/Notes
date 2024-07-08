#exam 
## VLANs
- extended range VLANs are stored in running-config, not written to vlan.dat
- normal range VLANs are stored in flash (vlan.dat)
### Inter-VLAN Routing
- legacy router
- router-on-a-stick
	- uses subinterfaces and dot1Q encapsulation
	- does not scale well past 50 VLANs
- layer 3 switch
	- uses multiple SVIs (switch virtual interfaces) for each VLAN
	- `no switch` creates routed port
	- traffic is routed via internal VLAN interfaces
### STP
- **PortFast** bypasses listening and learning
	- goes from blocking to forwarding
	- only on ports with end devices (BPDUs are not recieved)
- removes frame loops and give redundancy
- prevents looping for broadcast, multicast, and unknown multicast
- **root ports** best route to root bridge
### EtherChannel
- LACP `active/passive/on` (aka 802.3ad (fuck you IEEE))
- PAgP `desirable/auto/on`
- STP recalculation is not needed on a failed link
- allowed VLANs, trunking, and the native VLAN must match
- load balancing
	- src IP to dst IP
	- src MAC to dst MAC
-  