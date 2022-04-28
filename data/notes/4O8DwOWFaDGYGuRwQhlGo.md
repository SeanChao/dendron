
> [CLI reference](https://caddyserver.com/docs/command-line)

## Docker

⚠ Don't forget to map ports or use host network!

```sh
docker run caddy caddy file-server
```

## Caddyfile

```Caddyfile

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

## Reverse Proxy

```
route /stgui/* {
  uri strip_prefix /stgui
  reverse_proxy syncthing:8384
}
```
