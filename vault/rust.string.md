---
id: bFGSO6IQzvd38BNuz0QTg
title: String
desc: ''
updated: 1631242404735
created: 1629790933556
---

[String](https://doc.rust-lang.org/std/string/struct.String.html)

```rust
pub fn ends_with<'a, P>(&'a self, pat: P) -> bool
where
    P: Pattern<'a>,
    <P as Pattern<'a>>::Searcher: ReverseSearcher<'a>,
```

Returns `true` if the given pattern matches a suffix of this string slice.

```rust
assert_eq!("bar:foo".strip_suffix(":foo"), Some("bar"));
assert_eq!("bar:foo".strip_suffix("bar"), None);
assert_eq!("foofoo".strip_suffix("foo"), Some("foo"));

assert_eq!("11foo1bar11".trim_end_matches('1'), "11foo1bar");
assert_eq!("123foo1bar123".trim_end_matches(char::is_numeric), "123foo1bar");

let x: &[_] = &['1', '2'];
assert_eq!("12foo1bar12".trim_end_matches(x), "12foo1bar");
```

Turn `Vec<u8>` into `String`: `str::from_utf8(buf)`
