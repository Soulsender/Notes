- VLAN 1 is reserved for untagged traffic (data that does not have a VLAN tag) which is also called native VLAN
- native VLANs must be the same on both ends of switches
- all trunks must have native VLANs
- native VLANs send untagged trafffic
- if a the VLAN that a port is associated with is deleted, the port goes inactive
#### DTP
- `desirable` actively tries to make the interface a trunk
- `auto` makes the interface be able to be a trunk, but does not do so explicitly
![[../../attachments/image/IOS Commands-1706632306369.jpeg]]