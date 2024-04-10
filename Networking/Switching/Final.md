### Dynamic Trunking (DTP)
- `switchport nonegotiate` 
- default dynamic auto
### Spanning Tree (STP)
- lower bridge priority is preferable
- if priority is same; lowest MAC wins
- **priority** = 32768 + extended sys ID
- **portfast** = blocking >>> forwarding

| STP Version | Desc                                                           |
| ----------- | -------------------------------------------------------------- |
| STP         | original, aka CST                                              |
| PVST+       | seperate 802.1D ST instance for each VLAN                      |
| RSTP        | faster version of STP                                          |
| Rapid PVST+ | seperate 802.1w instance per VLAN, has BPDU guard and portfast |
| MSTP        | IEEE maps multiple                                             |
| MST         | cisco version of MSTP, combines VLANs into TSTP instance       |
### Etherchannel
- LACP (act/pas) / PAgP (aut/des)
- SU = in use