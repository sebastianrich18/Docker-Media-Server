# Docker-Media-Server
Jellyfin Media server with Sonarr, Radarr, qBittorrent (with vpn) and jackett.

# VPN Setup

# File Structure
 * downloads
    * where files downloaded from qBittorrent are stored
 * config
    * where configuration for each program is located, each in their own folders
    * PUT WIREGUARD CONFIG IN `config/wireguard`
 * completed
    * where sonarr and radarr will move your media from downloads. This will be where jellyfin looks for media.
# Starting
 * After configuring, simply `cd` into the cloned directory and run `docker-compose up -d`

