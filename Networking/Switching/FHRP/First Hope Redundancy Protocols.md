#fhrp
- two routers can share a virtual IP to give the illusion of a single router
### Hot Standby Router Protocol (HSRP)
- cisco proprietary
- active and standby device
- standby monitors active router to see if it goes down
- IPv6 version exists as well
### Virtual Router Redundancy Protocol v2 (VRRPv2)
- non-proprietary protocol
- assigns responsibility to one or more routers
- allows multiple routers to use same virtual IPv4 address
- VRRPv3 is used for IPv6
	- multivendor, and scalable
### Gateway Load Balancing Protocol (GLBP)
- cisco proprietary
- provides load balancing
- IPv6 version also exists
### ICMP Router Discovery Protocol (IRDP)
- legacy FHRP