sudo iptables -S
  
  // sudo apt-install iptables-persistent
  
 sudo iptables -A INPUT -p icmp -m icmp --icmp-type 8 -j DROP
 sudo iptables -A OUTPUT -p icmp -m icmp --icmp-type 0 -j DROP
