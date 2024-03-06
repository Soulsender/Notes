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