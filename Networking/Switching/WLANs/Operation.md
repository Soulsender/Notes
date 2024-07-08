#wlans 
### BSS
- single AP interconnecting all wireless clients
- uses BSSID, associated with only one AP
### ESS
- two or more BSSs can be joined
- multiple APs
- uses SSID (or ESSID)
### CSMA/CA
1. client listens to see if channel is idle
2. sends request to send (RTS)
3. receives clear to send (CTS)
	1. if client does not receive CTS will wait random time
4. transmits data
5. all transmissions are ack; if no ack assumes collision occurred - restarts
### CAPWAP
- enables WLC to manage multiple APs and WLANs
- UDP 5246/5247 (control/encap)
- DTLS encryption
### FlexConnect
- configure and control without WAN link
- **connected mode**
	- WLC is reachable
	- send traffic through CAPWAP tunnel
- **standalone**
	- WLC is unreachable
	- no CAPWAP
	- FlexConnect assumes some WLC functions