I'll make this readme... Some day...

Stuff to do before/after starting docker-compose:

BEFORE
- move config files from repo to <CONFIG>
- change .env file
- chmod 600 <CONFIG>/acme/acme.json
- check config for wildcard cert generation and add DNS redirections (wildcard or for every service)
- add vpn.conf in <CONFIG>/vpn
- add PLEX_CLAIM 

AFTER
- chown -R 1000:1000 <downloads>
- change ports in rutorrent VPN and restart it (2 ports for DHT and connections)
- create admin account in portainer
- create account in nextcloud
- setup plex
- connect tautulli to plex
- change deluge password
- config heimdall for everything (URLs for APIs are http://service:port [eg. http://sonarr:8989])
- config sonarr, radarr, jackett, bazarr 
    - Host for client rutorrent-VPN: vpn
    - Host for sonarr: sonarr, radarr: radarr
    - URL for jackett: http://jackett:9117/torznab/all/api