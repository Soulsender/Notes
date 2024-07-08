#spanning-tree 
#### Roles
- **root ports** - the best port to reach the bridge
- **designated port** - port with best route to root bridge on a link
- **non-designated ports** - all other ports that are in a blocking state
#### States
- **disabled** - shutdown port
- **blocking** - port that is blocking traffic
- **listening** - not forwarding and not learning MACs
- **learning** - not forwarding; learning MACs
- **forwarding** - send/receive traffic normally