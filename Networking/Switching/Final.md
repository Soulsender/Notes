### Dynamic Trunking (DTP)
- `switchport nonegotiate` 
- default dynamic auto
### Spanning Tree (STP)
- lower bridge priority is preferable
- if priority is same; lowest MAC wins
- **priority** = 32768 + extended sys ID
- **portfast** = blocking >>> forwarding

| STP Version | Desc                                                                       |
| ----------- | -------------------------------------------------------------------------- |
| STP         | original, aka CST                                                          |
| PVST+       | seperate 802.1D ST instance for each VLAN                                  |
| RSTP        | faster version of STP                                                      |
| Rapid PVST+ | seperate 802.1w instance per VLAN, has BPDU guard and portfast; cisco prop |
| MSTP        | IEEE maps multiple                                                         |
| MST         | cisco version of MSTP, combines VLANs into TSTP instance                   |
### Etherchannel
- LACP (act/pas) / PAgP (aut/des)
- SU = in use
#### DHCPv6
- stateful = `A=0 O=0 M=1`
- stateless = `A=1 O=1 M=0`
- relay = `ipv6 dhcp relay dest {addr}`
#### FHRP

| Protocol           | Desc                                 |
| ------------------ | ------------------------------------ |
| HSRP (Hot Standby) | active & standby devices; cisco prop |
| VRRP               | virtual routers; open source         |
| GLBP               | load balances; cisco prop            |
### Dynamic ARP Inspection
- requires DHCP snooping global
- verifies IP-to-MAC
### Static Routing

| Letter | Desc                   |
| ------ | ---------------------- |
| L      | address for router int |
| C      | directly connected     |
| S      | static route           |
| O      | dynamic route          |
| *      | default route          |
