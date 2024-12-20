# sebsk's homeserver

This repo hosts rewrite of my personal homeserver. It assumes five different machines to different tasks:

- Reverse proxy machine: the one and only.
- Storage machine: all the stuff that has heavy lifting with data. It has qBitTorrent and *arr services. Serves them via NFS.
- Media machine: Nextcloud, Jellyfin, Immich.
- Security machine: Vaultwarden, Zoneminder, Homeassistant.
- Services machine: Everything else that doesn't belong to all other three (e.g Paperless-ngx).

Every machine except reverse proxy has nginx which routes the traffic to corresponding dockers.

All the machines have internal network with reverse proxy machine.

All the machines, except reverse proxy machine are connected with another internal network, which is for storage.

In future i plan to move from Docker to Kubernetes.
