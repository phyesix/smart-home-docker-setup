Environments

- homeassistant
- watchtower
- wireguard
- transmission
- adguard
- cloudflared
- portainer
- homebox
- bazarr
- calibre-web
- mqtt
- zigbee2mqtt
- duplicati
- qbittorrent
- jellyfin
- lidarr
- plex
- prowlarr
- radarr
- sonarr
- jdownloader-2
- nzbget
- speedtest-tracker
- speedtest-database
- nginx
- code-server
- chromium

nano /etc/network/interfaces

```
# Network is managed by Network manager
auto lo
iface lo inet loopback
pre-up ip link set eth0 promisc on
# macvlan for docker
auto macvlan0
iface macvlan0 inet manual
    pre-up ip addr add 10.100.0.5/16 dev macvlan0
    up ip link set macvlan0 up
    post-up ip route add 10.100.1.10/32 dev macvlan0
    post-up ip route add 10.100.1.11/32 dev macvlan0
    post-up ip route add 10.100.1.12/32 dev macvlan0
    post-up ip route add 10.100.1.13/32 dev macvlan0
    post-up ip route add 10.100.1.14/32 dev macvlan0
    post-up ip route add 10.100.1.15/32 dev macvlan0
    post-up ip route add 10.100.1.16/32 dev macvlan0
    post-up ip route add 10.100.1.17/32 dev macvlan0
    post-up ip route add 10.100.1.18/32 dev macvlan0
    post-up ip route add 10.100.1.19/32 dev macvlan0
    post-up ip route add 10.100.1.20/32 dev macvlan0
    post-up ip route add 10.100.1.21/32 dev macvlan0
    post-up ip route add 10.100.1.22/32 dev macvlan0
    post-up ip route add 10.100.1.23/32 dev macvlan0
    post-up ip route add 10.100.1.24/32 dev macvlan0
    post-up ip route add 10.100.1.25/32 dev macvlan0
    post-up ip route add 10.100.1.26/32 dev macvlan0
    post-up ip route add 10.100.1.27/32 dev macvlan0
    post-up ip route add 10.100.1.28/32 dev macvlan0
    post-up ip route add 10.100.1.29/32 dev macvlan0
    post-up ip route add 10.100.1.30/32 dev macvlan0
    post-up ip route add 10.100.1.31/32 dev macvlan0
    post-up ip route add 10.100.1.32/32 dev macvlan0
    post-up ip route add 10.100.2.10/32 dev macvlan0
    post-up ip route add 10.100.2.11/32 dev macvlan0
```
    post-up ip route add 10.100.2.12/32 dev macvlan0
    post-up ip route add 10.100.2.13/32 dev macvlan0
    post-up ip route add 10.100.2.14/32 dev macvlan0
    post-up ip route add 10.100.2.15/32 dev macvlan0
