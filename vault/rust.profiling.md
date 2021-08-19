---
id: 9pKt2g7tu9gfqT6ha9p98
title: Profiling
desc: ''
updated: 1629350038596
created: 1629349636917
---

Release build with debug info:

```toml
[profile.release]
opt-level = 3
debug = 1
```

## Valgrind DHAT

    valgrind --tool=dhat ./prog

