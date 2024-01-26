```
PORT      STATE SERVICE  REASON  VERSION
22/tcp    open  ssh      syn-ack OpenSSH 7.9p1 Debian 10+deb10u2 (protocol 2.0)
| ssh-hostkey: 
|   2048 bd:96:ec:08:2f:b1:ea:06:ca:fc:46:8a:7e:8a:e3:55 (RSA)
| ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDTTsq+a0RxMS1DLjWFk0IndtbAH7nXVGiY9aoSiRpo0DtgIdqXpzkjTXbCM/Zcm7K2IpOmE85vQZpcOTlHDSzaRfqxMEUWFXlCoKoSAI6RKh8AV9zB0ZiHD+DrRlm20nzKh9DHfJAf7QmxVluH/5P8ystOOWfcyn/Dfo8kP6+Dc5T5WWfTuodst45cSKWfSAyka/gcU/HMw5QTGmEIIZYc0ro2PU1roC0/uGqx3Ms+ztneXf4P66bGGq47/mWAyvRLQvdbCZzkUQOoYoi7lqi+AM4Yssw91Z/pQc90fkWUUgRT7dmkpz3KLaHYD06iDoOuLbWPEIpyzFk9v1gAR+Q3
|   256 56:32:3b:9f:48:2d:e0:7e:1b:df:20:f8:03:60:56:5e (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBNsVRVQLTyQL2IDtWvOo4P3UtG7Xen5vavIS5yS1Bg+RdwkKVUkPh8B8m1BA0h3qBvoPXTnW2BH9oUv6WnswP60=
|   256 95:dd:20:ee:6f:01:b6:e1:43:2e:3c:f4:38:03:5b:36 (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIMnrkcxZcAlbLRzcQ0uhebcMa6PvIEE+2XjB4/HUrvy6
80/tcp    open  http     syn-ack Apache httpd 2.4.38 ((Debian))
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-server-header: Apache/2.4.38 (Debian)
|_http-title: Bolt - Installation error
111/tcp   open  rpcbind  syn-ack 2-4 (RPC #100000)
| rpcinfo: 
|   program version    port/proto  service
|   100000  2,3,4        111/tcp   rpcbind
|   100000  2,3,4        111/udp   rpcbind
|   100000  3,4          111/tcp6  rpcbind
|   100000  3,4          111/udp6  rpcbind
|   100003  3           2049/udp   nfs
|   100003  3           2049/udp6  nfs
|   100003  3,4         2049/tcp   nfs
|   100003  3,4         2049/tcp6  nfs
|   100005  1,2,3      44021/tcp   mountd
|   100005  1,2,3      51672/udp6  mountd
|   100005  1,2,3      51847/tcp6  mountd
|   100005  1,2,3      57463/udp   mountd
|   100021  1,3,4      33295/tcp   nlockmgr
|   100021  1,3,4      43583/tcp6  nlockmgr
|   100021  1,3,4      56230/udp   nlockmgr
|   100021  1,3,4      59499/udp6  nlockmgr
|   100227  3           2049/tcp   nfs_acl
|   100227  3           2049/tcp6  nfs_acl
|   100227  3           2049/udp   nfs_acl
|_  100227  3           2049/udp6  nfs_acl
2049/tcp  open  nfs_acl  syn-ack 3 (RPC #100227)
8080/tcp  open  http     syn-ack Apache httpd 2.4.38 ((Debian))
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
| http-open-proxy: Potentially OPEN proxy.
|_Methods supported:CONNECTION
|_http-server-header: Apache/2.4.38 (Debian)
|_http-title: PHP 7.3.27-1~deb10u1 - phpinfo()
33295/tcp open  nlockmgr syn-ack 1-4 (RPC #100021)
37775/tcp open  mountd   syn-ack 1-3 (RPC #100005)
41143/tcp open  mountd   syn-ack 1-3 (RPC #100005)
44021/tcp open  mountd   syn-ack 1-3 (RPC #100005)
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

```