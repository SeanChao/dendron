---
id: zq90O0PuaZoF5QghaJyNA
title: Cache
desc: ''
updated: 1630133485555
created: 1629255926895
---

Examples to cache dependencies in GitHub actions.

## NPM

```yml
- name: Cache NPM dependencies
  uses: actions/cache@v2
  with:
    path: |
      **/node_modules
    key: ${{ runner.os }}-${{ hashFiles('**/yarn.lock') }}
```

## Rust/Cargo

```yml
- uses: actions/cache@v2
  with:
    path: |
      ~/.cargo/bin/
      ~/.cargo/registry/index/
      ~/.cargo/registry/cache/
      ~/.cargo/git/db/
      target/
    key: ${{ runner.os }}-cargo-${{ hashFiles('**/Cargo.lock') }}
```
