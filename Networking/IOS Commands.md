### ACLs
- `permit` allow group
- `deny` deny group
### VLANs
- `switch mode access` set to not trunk (STATIC)
- `switchport mode trunk` enable trunking on the interface (STATIC)
- `switchport nonegotiate` stops interface from sending DTP frames (DYNAMIC)
- `switchport mode dynamic auto/desirable` enables DTP (DYNAMIC)
- `switch access vlan 10` set port to be used for VLAN 10
- `vlan 10` switch to vlan 10 config
- `name {name}` set vlan name
- `no switchport trunk allowed vlan` remove allowed VLANs and reset native VLAN trunk
- `switchport trunk native vlan 99` change native vlan to vlan 99
- `switchport trunk allowed vlan 10,20,30` sets allowed vlans
- `mls qos trust cos` does something with QoS for VoIP idk what lol
- `swi voice vlan 150` puts voice stuff on vlan 150
### Inter-VLAN Routing
- `int g0/0.10` create subinterface
- `encapsulation dot1Q 10` sets encapsulation type to 802.1Q
- `no switchport` make port a routed port (layer 2 int)
### OSPF
- `ip ospf priority {priority}` explicitly state priority
- `ip ospf {cost}` explicitly states cost
- `ip ospf {pid} area {area}` set ospf on area interface
- `ip ospf network point-to-point` make interface point to point
- `ip ospf {hello/dead}-interval {10/40}` change hello/dead interval
- `router ospf 10` enter ospf config
- `router-id {rid}` explicitly state RID
- `network {ip}` set network statement
- `clear ip ospf process` restart ospf process
- `passive-interface loop1` set loop1 as passive interface
- `auto-cost reference-bandwidth {1000/10000}` set auto cost (fa/gi)
- `default-information originate` sets ospf default route (used with `ip route`)
### SSH
- `ip domain name example.com`
- `crypto key generate rsa (general-keys modulus 512)`
- `username admin secret cisco`
- `line vty 0 15`
- `login local`
- `transport input ssh`
### Navigation
- `enable` enter priv EXEC (`en`)
- `disable` enter user EXEC
- `configure terminal` global mode (`conf t`)
- `end` enter from any mode to priv EXEC mode
### Misc
- `description {description}` give item description
- `banner motd {banner}` create a warning banner
- `traceroute {ip}` traceroute ip address 
- `no {command}` delete command specified
### Keybindings
- Ctrl + C -> cancel current task, clear line
- Ctrl + Shift + 6 -> cancel "translating" task
### Show (`sh`)
- `show version` get version and system info
- `show interface status` show all interfaces
- `show ip interface brief` show ip address information
- `show running-config` show current config
- `show startup-config` show boot config
- `show ip ospf neighbor` show ospf neighbour details
- `show ip protocols` show ospf RID
- `show ip route` show routing table
- `show vlan` show vlan table
- `show interface trunk` show trunk interfaces
### Config (`conf`)
- `line console 0` enter **console** config interface (`line con 0`)
- `line vty 0 15` enter **virtual terminal** config interface (for SSH, Telnet)
- `interface vlan 1` enter **vlan** config interface
- `interface FastEthernet 0/1` enter ethernet config interface (`int fa 0/1`)
- `no shutdown` enable virtual interface
- `copy running-config startup-config` save running & startup config files
- `erase startup-config` erases startup-config
- `reload` restore to startup-config (device will go offline briefly)
### Passwords
- `password {password}` change user EXEC password (used in `line console 0` and `line vty 0 15`)
- `login` enable user EXEC password access
- `enable secret {password}` change priv EXEC password
- `enable password {password}` change priv EXEC unencrypted password
- `service password-encrypion` enable password encryption
### IP Addressing
- `ip address {192.168.1.20} {255.255.255.0}` set a manual ip address and subnet mask
- `ip default-gateway {192.168.0.254}` set the router address
- `show ip interface brief` show ip address information
- `ip route {network address to connect} {subnet mask} {ip of hop to network}`
	- ex. `192.168.10.0 255.255.255.0 209.165.200.225`
- `ip route {network address to connect} {subnet mask} {interface exit}`
	- ex. `192.168.10.0 255.255.255.0 G0/0/1`
- `ip default-gateway {router address}`
### IPv6
- `ipv6 address fe80::1 link-local`
- `ipv6 address 2001:db8::1/64`
- `ipv6 unicast-routing`

