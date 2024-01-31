--Start AP--
hostapd hostapd.conf

--Assign Gateway/Netmask--
ifconfig wlan1 up 192.168.1.1 netmask 255.255.255.0
route add -net 192.168.1.0 netmask 255.255.255.0 gw 192.168.1.1

--Start DNS Server--
dnsmasq -C dnsmasq.conf -d

--Internet Connection--
iptables --table nat --append POSTROUTING --out-interface eth0 -j MASQUERADE
iptables --append FORWARD --in-interface wlan1mon -j ACCEPT

echo 1 > /proc/sys/net/ipv4/ip_forward