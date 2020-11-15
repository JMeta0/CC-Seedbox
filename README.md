Stuff to do before/after starting docker-compose:

BEFORE
- move config files from repo to CONFIG
- change .env file
- add vpn.conf in CONFIG/vpn
- check /dev for scrutiny and add/remove disks to match

AFTER
- chown -R user:user downloads folder
- change ports in rutorrent VPN rtorrent.rc and restart it
- create admin account in portainer
- connect tautulli to plex
- change deluge password
- config heimdall for everything (URLs for APIs are http://service:port [eg. http://sonarr:8989])
- config sonarr, radarr, jackett, bazarr 
    - Host for client rutorrent-VPN: vpn
    - Host for sonarr: sonarr, radarr: radarr
    - URL for jackett: http://jackett:9117/torznab/all/api
