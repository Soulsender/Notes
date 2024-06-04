#ospf #routing 
#### Down State
- no hello packets
- router sends hello
- transition to init state
#### Init State
- hello packets received by neighbour
- contains RID of sending router
- transition to two-way state
#### Two Way State
- comms are bidirectional
- on multiaccess, router elect DR and BDR
- transition to ExStart
#### ExStart
- on point to point networks, two routers decide which router will init the DBD packet
#### Exchange
- exchange DBD
- if not same, will transition to loading
#### Loading
- LSRs and LSUs are used to gain additional route info
- routes are process with SPF algorithm
#### Full
- fully inited