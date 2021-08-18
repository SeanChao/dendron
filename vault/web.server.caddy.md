---
id: 4O8DwOWFaDGYGuRwQhlGo
title: Caddy
desc: ''
updated: 1629257311188
created: 1629256733447
---

> [CLI reference](https://caddyserver.com/docs/command-line)

## Docker

⚠ Don't forget to map ports or use host network!

```sh
docker run caddy caddy file-server
```

## File server

```sh
caddy file-server
	[--root <path>]
	[--listen <addr>]
	[--domain <example.com>]
	[--browse]
	[--templates]
	[--access-log]

docker run --network host -v $PWD:/srv caddy caddy file-server --root /srv --listen localhost:2333 -browse
```


