#spanning-tree 
- allows switch port to bypass listening and learning states and go immediately to forwarding
- immediately goes from blocking to forwarding
- only configured on ports with end devices
- BPDUs are not received on PortFast port
- supports DHCP
	- without PortFast, devices will issue DHCP requests before port is in forwarding state