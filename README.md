# sebsk's homeserver

This repo hosts rewrite of my personal homeserver. It assumes four different machines to different tasks:

- Reverse proxy machine: it just contains reverse proxy (haproxy) to other machines
- Storage machine: the stuff that is important to have backups of
- Matrix machine: bridge of all stuff that i don't really need, but frens use - Facebook Messenger, Whatsapp, Instagram chats, Telegram
- Dockers machine: It contains all the apps that i use, each isolated in docker, for now it's about 10-13 apps like Paperless-ngx, Nextcloud, PhotoPrism etc.

Dockers machine uses the storage machine for the stuff that really needs it (e.g Nextcloud user files). In future i plan to move from Docker to Kubernetes.

## TODO

### Matrix:

- [ ]  Syncv3 account and database creation
