### Dynamic Trunking (DTP)
- `switchport nonegotiate` 
- default dynamic auto
### Spanning Tree (STP)
- lower bridge priority is preferable
- if priority is same; lowest MAC wins
- priority = 32768 + extended sys ID

| STP Version | Desc                                      |
| ----------- | ----------------------------------------- |
| STP         | original, aka CST                         |
| PVST+       | seperate 802.1D ST instance for each VLAN |
| RSTP        | faster version of STP                     |
| Rapid PVST+ | seperate 802.1w instance per VLAN         |
| MSTP        | IEEE maps multiple                        |
|             |                                           |
