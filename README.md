Environments

1. Nginx Proxy Manager
2. Home Assistant
3. PiHole
4. Wireguard
5. Transmission
6. Adguard
7. Cloudflared
8. Portainer
9. Homebox

...

nano /etc/network/interfaces

# Network is managed by Network manager
auto lo
iface lo inet loopback
pre-up ip link set eth0 promisc on
# macvlan for docker
auto macvlan0
iface macvlan0 inet manual
    pre-up ip link set eth0 promisc on
    pre-up ip link add macvlan0 link eth0 type macvlan mode bridge
    pre-up ip link set macvlan0 promisc on
    pre-up ip addr add 10.0.0.5/16 dev macvlan0
    up ip link set macvlan0 up
    post-up ip route add 10.0.1.10/32 dev macvlan0
    post-up ip route add 10.0.1.11/32 dev macvlan0
    post-up ip route add 10.0.1.12/32 dev macvlan0
    post-up ip route add 10.0.1.13/32 dev macvlan0
    post-up ip route add 10.0.1.14/32 dev macvlan0
    post-up ip route add 10.0.1.15/32 dev macvlan0
    post-up ip route add 10.0.1.16/32 dev macvlan0
    post-up ip route add 10.0.1.17/32 dev macvlan0
    post-up ip route add 10.0.2.10/32 dev macvlan0
    post-up ip route add 10.0.2.11/32 dev macvlan0
