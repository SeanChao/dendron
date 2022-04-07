---
id: 34HTG9klr3NzTjkUghbvJ
title: Ssh
desc: ''
updated: 1630932083347
created: 1630931658841
---

```ssh
Host example.com
  HostName example.com
  Port 2333
  User shinji
  IdentityFile ~/.ssh/id_rsa # Use private key
```

On the target machine: add the public key into `~/.ssh/authorized_keys`
