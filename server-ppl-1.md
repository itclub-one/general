# iptables-persistent 
to restore iptable after restart, the content of the iptable is basically NAT F>

# netplans
The WAN interface is DHCPv4 while LAN interface is set manually and override th>
doesn't become default route

# iptables
Controlling LAN network
## To block destination with port
iptables -I FORWARD -i enp5s0 -p tcp --dport 8000 -j DROP

## To block destination ip
iptables -I FORWARD -i enp5s0 -d 1.1.1.1 -j REJECT
