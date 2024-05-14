- only happen on multiarea (router serial) networks, not point 2 point (ethernet)
- highest interface OSPF priority wins election (0-255)
- default priority is 1
- if priority is tied - highest RID wins election
#### DRs and BDRs
- used to reduce LSA traffic
- DROTHERs are routers that are not the BR or BDR