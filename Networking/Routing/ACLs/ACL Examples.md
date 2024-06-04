#acls
### Extended ACL 1:
- Explicitly block FTP access to the Enterprise Web Server from the internet.
- No ICMP traffic from the internet should be allowed to any hosts on HQ LAN 1
- Allow all other traffic.
```
access-list 101 deny tcp any host 192.168.1.70 eq ftp
access-list 101 deny icmp any 192.168.1.0 0.0.0.63
access-list 101 permit ip any any
```

#### Extended ACL 2:
- No hosts on HQ LAN 1 should be able to access the Branch Server.
- All other traffic should be permitted.
```
access-list 111 deny ip any host 192.168.2.45
access-list 111 permit ip any any
```

#### Extended ACL 3:
```
ip access-list extended branch_to_hq
deny ip 192.168.2.0 0.0.0.31 192.168.1.0 0.0.0.63
deny ip 192.168.2.32 0.0.0.15 192.168.1.0 0.0.0.63
permit ip any any
```

#### Standard ACL 1:
- Create a named standard ACL. Use the name vty_block. The name of your ACL must match this name exactly.
- Only addresses from the HQ LAN 2 network should be able to access the VTY lines of the HQ router.
```
ip access-list standard vty_block
permit ip 192.168.1.64 0.0.0.7
```