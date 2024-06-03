### Example
- R1 joins routing domain
- sends EIGRP hello to all EIGRP ports
- R2 receives hello, adds R1 to neighbor table
- R2 sends update packet with all routes it knows
- R2 sends hello to R1
- R1 updates neighbor table with R2
