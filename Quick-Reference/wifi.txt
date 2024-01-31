
--Aircrack suite--
airmon-ng = manages network cards (airmon-ng start wlan0)
airodump-ng = detects devices and routers. take BSSID and channels. (airodump-ng --bssid --channel)
aireplay-ng = attack (--deauth -c [client mac] -a [AP mac] wlan0)
aircrack-ng = crack handshake (aircrack-ng network.cap -w [wordlist])

--ARP--
arp-scan = detects devices on the network (sudo arp-scan --interface=wlp59s0 --localnet)

--Random MAC Addressing--
OUI second bit will be: 
2 6 A E
