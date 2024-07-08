#linux #networking
#### Interface Naming
- hardware
	- `en` - ethernet
	- `wl` - wlan
	- `ww` - wwan (mobile)
- firmware/location
	- `oX` - on board device; X provided by firmware
	- `sX` - PCI slot X
	- `pXsZ` - PCI device on bus X slot Z
#### ip
- `ip link show` show interfaces and MACs
- `ip addr show ens3` show ip of interface
- `ip -s link show ens3` show performance of interface
- `ip (-6) route` show IPv4/(IPv6) routing table
#### nmcli
- `nmcli dev status` status of all network devices
- `nmcli con show --active` show active connections
- `nmcli con up static-enp3` bring up network connection
- `nmcli dev dis ens3` disconnect network (autoconnect will connect you back)
- `nmcli con add con-name eno2 type ethernet ifname eno2 ipv4.address 192.168.0.3 ipv4.gateway 192.168.0.1` add a new network connection


#### Misc Commands
- `ss -ta` troubleshoot ports and services


