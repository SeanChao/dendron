---
id: zq90O0PuaZoF5QghaJyNA
title: Cache
desc: ''
updated: 1629256024403
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
