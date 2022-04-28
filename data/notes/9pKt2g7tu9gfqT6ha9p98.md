
Release build with debug info:

```toml
[profile.release]
opt-level = 3
debug = 1
```

## Valgrind DHAT

    valgrind --tool=dhat ./prog
