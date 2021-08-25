---
id: uCa7YBe3JQFPWW0I0X4Nr
title: Notifications
desc: ''
updated: 1629772548624
created: 1629772257076
---

    PUBLISH __keyspace@0__:mykey del # notifies a key
    PUBLISH __keyevent@0__:del mykey # notifies an event

## Configuration

```text
K     Keyspace events, published with __keyspace@<db>__ prefix.
E     Keyevent events, published with __keyevent@<db>__ prefix.

# in redis.conf:
notify-keyspace-events Kx
```
