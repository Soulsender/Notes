#networking 
- ip routing tech
- uses forwarding info base (FIB) & adjacency table
### Operation
- routing table has routes from OSPF, EIGRP, etc.
- FIB is built from routing table
- adjacency table is maintained from layer 2 info
- when packets arrive, CEF uses FIB to determine best forwarding path
### FIB
- data structure for CEF
- optimized for speed