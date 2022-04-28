
## Daemon

Edit `/etc/default/docker`:

```sh
export HTTPS_PROXY="http://sean-laptop.local:1080"
export HTTP_PROXY="http://sean-laptop.local:1080"
```

## Client

Edit `~/.docker/config.json`

```json
{
  "proxies": {
    "default": {
      "httpProxy": "http://192.168.1.12:3128",
      "httpsProxy": "http://192.168.1.12:3128",
      "noProxy": "*.test.example.com,.example2.com,127.0.0.0/8"
    }
  }
}
```

## Reference

- https://docs.docker.com/config/daemon/systemd/
- https://docs.docker.com/network/proxy/#configure-the-docker-client
