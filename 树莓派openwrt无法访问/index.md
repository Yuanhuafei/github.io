# 树莓派openwrt无法访问






sudo ip link add mynet link eth0 type macvlan mode bridge
sudo ip addr add 192.168.50.248 dev mynet
sudo ip link set mynet up
sudo ip route add 192.168.50.3 dev mynet
sudo ip route del 192.168.50.0/24 dev eth0
sudo ip route del default
sudo ip route add 192.168.50.0/24 dev mynet
sudo ip route add default via 192.168.50.3 dev mynet;

