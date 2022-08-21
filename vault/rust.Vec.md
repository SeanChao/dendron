---
id: k39RuYAC7CdaMz6kejaTf
title: Vec
desc: ''
updated: 1661064114972
created: 1630726736756
---

[doc](https://doc.rust-lang.org/std/vec/struct.Vec.html)

Emptiness: `pub fn is_empty(&self) -> bool`

`Vec` can be used as a stack:

```rust
let v = Vec::new();
v.push(1);
let i = v.pop().unwrap();
```
