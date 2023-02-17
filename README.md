# Docker-Media-Server
Jellyfin Media server with Sonarr, Radarr, qBittorrent (with vpn) and jackett.

# VPN Setup
   I am using [dyonr's qBittorrent docker image](https://hub.docker.com/r/dyonr/qbittorrentvpn/) check that out for further qBittorrent/VPN support
   * Create a wireguard config and name it `wg0.conf`
   * Put this config file in `config/wireguard`

# File Structure
 * `downloads`
    * where files downloaded from qBittorrent are stored
 * `config`
    * where configuration for each program is located, each in their own folders
    * PUT WIREGUARD CONFIG IN `config/wireguard`
 * `completed`
    * where sonarr and radarr will move your media from downloads. This will be where jellyfin looks for media.
# Usage
 * After configuring, simply `cd` into the cloned directory and run `docker-compose up -d`
 * sonarr is hosted at `localhost:8989`
 * radarr is hosted at `localhost:7979`
 * qBittorrent is hosted at `localhost:8080`
 * jackett is hosted at `localhost:9117`
 * jellyfin is hosted at `localhost:8096`

