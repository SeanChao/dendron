
    PUBLISH __keyspace@0__:mykey del # notifies a key
    PUBLISH __keyevent@0__:del mykey # notifies an event

## Configuration

```text
K     Keyspace events, published with __keyspace@<db>__ prefix.
E     Keyevent events, published with __keyevent@<db>__ prefix.

A     All.

# in redis.conf:
notify-keyspace-events Kx
```

Watch events:

```sh
redis-cli --csv psubscribe '__key*__:*'
```
