---
version: "2.1"
services:
  demopc:
    image: lscr.io/linuxserver/webtop:ubuntu-mate
    container_name: demopc
    environment:
      - PUID=1000
      - PGID=1000
      - TZ=Europe/London
      - PASSWORD=P@ssword!
      - SUBFOLDER=/ #optional
      - KEYBOARD=en-us-qwerty #optional
      - TITLE=Webtop #optional
    volumes:
      - /home/demopc/config:/config
      - /var/run/docker.sock:/var/run/docker.sock
    ports:
      - 3001:3001
    shm_size: "2gb" #optional
    restart: unless-stopped