- STP
	- original
	- assumes one spanning tree instance for entire bridged network regardless of VLANs
- PVST+
	- cicso version of STP
	- provides separate spanning tree for each VLAN
	- supports PortFast
	- cisco default
- RSTP
	- faster newer version of STP
- Rapid PVST+
	- cisco version of RSTP
	- provides seperate instance of 802.1w per VLAN
	- suppors PortFast
- MSTP
	- maps multiple VLANs into same spanning tree instance
- MST
	- cisco version of MSTP
	- up to 16 instances of RSTP
	- combines VLANs with same phyical and logical topology into common RSTP instance
	- supports PortFast