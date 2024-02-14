## Steps
1. host sends RS
2. router responds with RA
3. host sends DHCPv6 SOLICIT
4. DHCPv6 server responds with ADVERTISE
5. host responds to DHCPv6 server
6. DHCPv6 server sends reply message
## Roles
#### DHCPv6 Server
- router provides stateless/stateful DHCPv6
#### DHCPv6 Client
- router interface acquires IPv6 from other DHCPv6 server
#### DHCPv6 Relay Agent
- router forwards DHCPv6 services when client and server are on different networks