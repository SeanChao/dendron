---
id: 34HTG9klr3NzTjkUghbvJ
title: Ssh
desc: ''
updated: 1649914034427
created: 1630931658841
---

## SSH Client Config File

```ssh
Host example.com
  HostName example.com
  Port 2333
  User shinji
  IdentityFile ~/.ssh/id_rsa # Use private key
```

On the target machine: add the public key into `~/.ssh/authorized_keys`

## Key Management

### Private Key Permissions

The private key should be owner read only (0400). ^pkp

See also: [[FS permissions|filesystem#Permissions]]
