---
id: 2sq996cqtzuvgkkb0oxaffi
title: Filesystem
desc: ''
updated: 1649912227593
created: 1649407295998
---

## Permissions

Permission string = direcotry(1) + owner, owning group, everyone else permissions

```
drwxr-xr-x
This is a directory
owner: read, add/remove files, enter the directory
```

### Octal Representation

rwx represent a bit respectively.

e.g, r--rw-rwx = 100110111 = 0467

## APIs

mkdir

![[python.fs#directories]]
