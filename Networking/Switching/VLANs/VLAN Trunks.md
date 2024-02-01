- vlan1 is reserved for untagged traffic (data that does not have a VLAN tag) which is also called native vlan
- native vlans must be the same on both ends of switches
- all trunks must have native vlans
- native vlans send untagged trafffic
#### DTP
- `desirable` actively tries to make the interface a trunk
- `auto` makes the interface be able to be a trunk, but does not do so explicitly
![[../../attachments/image/IOS Commands-1706632306369.jpeg]]