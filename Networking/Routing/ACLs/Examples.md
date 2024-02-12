### Extended ACL 1:
```
access-list 101 deny tcp any host 192.168.1.70 eq ftp
access-list 101 deny icmp any 192.168.1.0 0.0.0.63 echo
access-list 101 permit ip any any
```
