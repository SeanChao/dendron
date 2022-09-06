
## Compose File

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

## CLI

```text
  -f, --file FILE             Specify an alternate compose file
                              (default: docker-compose.yml)
```
