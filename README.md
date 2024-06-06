Environments

- mqtt:         		5.10
- zigbee2mqtt   		5.11
- homeassistant 		5.12
- watchtower    		5.13
- adguard       		5.14
- portainer     		5.15
- homebox       		5.16
- calibre       		5.17
- calibre-web   		5.18
- duplicati     		5.19
- qbittorrent   		5.20
- jdownloader-2 		5.21
- jellyfin      		5.22
- lidarr        		5.23
- prowlarr      		5.24
- radarr      			5.25
- sonarr      			5.26
- bazarr      			5.27
- readarr      			5.28
- feedropolis   		5.29
- rssbridge     		5.30
- speedtest-tracker     5.31
- airsonic-advanced     5.32
- apprise-api     		5.33
- booksonic-air    		5.34
- spotube     			5.35
- headphones     		5.36
- nextcloud     		5.37
- pwndrop     			5.38
- syncthing     		5.39
- ubooquity     		5.40
- changedetection     	5.41

- nginx     			5.100
- code-server     		5.101
- chromium     			5.102
- firefox     			5.103
- browser-chrome     	5.104
- playwright-chrome     5.105
- openvscode-server     5.106
- pg_db     			5.107


```
nano /etc/network/interfaces
```

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
    post-up ip route add 10.100.5.10/32 dev macvlan0
    post-up ip route add 10.100.5.11/32 dev macvlan0
    post-up ip route add 10.100.5.12/32 dev macvlan0
    post-up ip route add 10.100.5.13/32 dev macvlan0
    post-up ip route add 10.100.5.14/32 dev macvlan0
    post-up ip route add 10.100.5.15/32 dev macvlan0
    post-up ip route add 10.100.5.16/32 dev macvlan0
    post-up ip route add 10.100.5.17/32 dev macvlan0
    post-up ip route add 10.100.5.18/32 dev macvlan0
    post-up ip route add 10.100.5.19/32 dev macvlan0
    post-up ip route add 10.100.5.20/32 dev macvlan0
    post-up ip route add 10.100.5.21/32 dev macvlan0
    post-up ip route add 10.100.5.22/32 dev macvlan0
    post-up ip route add 10.100.5.23/32 dev macvlan0
    post-up ip route add 10.100.5.24/32 dev macvlan0
    post-up ip route add 10.100.5.25/32 dev macvlan0
    post-up ip route add 10.100.5.26/32 dev macvlan0
    post-up ip route add 10.100.5.27/32 dev macvlan0
    post-up ip route add 10.100.5.28/32 dev macvlan0
    post-up ip route add 10.100.5.29/32 dev macvlan0
    post-up ip route add 10.100.5.30/32 dev macvlan0
    post-up ip route add 10.100.5.31/32 dev macvlan0
    post-up ip route add 10.100.5.32/32 dev macvlan0
    post-up ip route add 10.100.5.33/32 dev macvlan0
    post-up ip route add 10.100.5.34/32 dev macvlan0
    post-up ip route add 10.100.5.35/32 dev macvlan0
    post-up ip route add 10.100.5.36/32 dev macvlan0
    post-up ip route add 10.100.5.37/32 dev macvlan0
    post-up ip route add 10.100.5.38/32 dev macvlan0
    post-up ip route add 10.100.5.39/32 dev macvlan0
    post-up ip route add 10.100.5.40/32 dev macvlan0
    post-up ip route add 10.100.5.41/32 dev macvlan0
    post-up ip route add 10.100.5.100/32 dev macvlan0
    post-up ip route add 10.100.5.101/32 dev macvlan0
    post-up ip route add 10.100.5.102/32 dev macvlan0
    post-up ip route add 10.100.5.103/32 dev macvlan0
    post-up ip route add 10.100.5.104/32 dev macvlan0
    post-up ip route add 10.100.5.105/32 dev macvlan0
    post-up ip route add 10.100.5.106/32 dev macvlan0
    post-up ip route add 10.100.5.107/32 dev macvlan0
```
