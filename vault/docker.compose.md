---
id: NjmLXR2FTwuqZG4PMPoZM
title: Compose
desc: ''
updated: 1630770527675
created: 1630681664800
---

Reference: [compose-file-v3](https://docs.docker.com/compose/compose-file/compose-file-v3)

Template

```yml
version: '3'

services:
  caddy:
    restart: on-failure
    image: 'caddy'
    volumes:
      - './caddy/Caddyfile:/etc/caddy/Caddyfile'
    network_mode: host
  mirror:
    build:
      context: .
      dockerfile: Dockerfile
      command: ['-p', '3000']
  tg:
    restart: on-failure
    image: telegrammessenger/proxy
    ports:
      - '2333:443'
    env_file:
      - tg.env
```
