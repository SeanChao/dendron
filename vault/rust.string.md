---
id: bFGSO6IQzvd38BNuz0QTg
title: String
desc: ''
updated: 1629790984572
created: 1629790933556
---

```
pub fn ends_with<'a, P>(&'a self, pat: P) -> bool
where
    P: Pattern<'a>,
    <P as Pattern<'a>>::Searcher: ReverseSearcher<'a>,
```

Returns `true` if the given pattern matches a suffix of this string slice.
