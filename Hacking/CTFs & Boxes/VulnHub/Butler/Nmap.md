```
PORT      STATE SERVICE       REASON  VERSION
135/tcp   open  msrpc         syn-ack Microsoft Windows RPC
139/tcp   open  netbios-ssn   syn-ack Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds? syn-ack
7680/tcp  open  pando-pub?    syn-ack
8080/tcp  open  http          syn-ack Jetty 9.4.41.v20210516
|_http-favicon: Unknown favicon MD5: 23E8C7BD78E8CD826C5A6073B15068B1
| http-robots.txt: 1 disallowed entry 
|_/
|_http-server-header: Jetty(9.4.41.v20210516)
|_http-title: Site doesn't have a title (text/html;charset=utf-8).
49664/tcp open  msrpc         syn-ack Microsoft Windows RPC
49665/tcp open  msrpc         syn-ack Microsoft Windows RPC
49666/tcp open  msrpc         syn-ack Microsoft Windows RPC
49667/tcp open  msrpc         syn-ack Microsoft Windows RPC
49668/tcp open  msrpc         syn-ack Microsoft Windows RPC
49669/tcp open  msrpc         syn-ack Microsoft Windows RPC
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: -2s
| nbstat: NetBIOS name: BUTLER, NetBIOS user: <unknown>, NetBIOS MAC: 08:00:27:30:37:21 (Oracle VirtualBox virtual NIC)
| Names:
|   BUTLER<00>           Flags: <unique><active>
|   WORKGROUP<00>        Flags: <group><active>
|   BUTLER<20>           Flags: <unique><active>
| Statistics:
|   08 00 27 30 37 21 00 00 00 00 00 00 00 00 00 00 00
|   00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
|_  00 00 00 00 00 00 00 00 00 00 00 00 00 00
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 54171/tcp): CLEAN (Couldn't connect)
|   Check 2 (port 8773/tcp): CLEAN (Couldn't connect)
|   Check 3 (port 18579/udp): CLEAN (Timeout)
|   Check 4 (port 33693/udp): CLEAN (Failed to receive data)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked
| smb2-security-mode: 
|   2.02: 
|_    Message signing enabled but not required
| smb2-time: 
|   date: 2022-11-03T16:28:49
|_  start_date: N/A

```