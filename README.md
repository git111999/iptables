sudo iptables -S
  
  // sudo apt-install iptables-persistent
  sudo iptables-save > /etc/iptables/rules.v4
  sudo iptables-save > /etc/iptables/rules.v6
  
 sudo iptables -A INPUT -p icmp -m icmp --icmp-type 8 -j DROP
 sudo iptables -A OUTPUT -p icmp -m icmp --icmp-type 0 -j DROP
 
 // nftables ?
