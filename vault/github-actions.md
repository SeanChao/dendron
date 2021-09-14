---
id: vLN66cbj18kIA9aNMw4MV
title: GitHub Actions
desc: ''
updated: 1631535602526
created: 1629255661366
---

Github actions snippets.

[Syntax reference](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions)

```yml
jobs:
  job1:
  job2:
    needs: job1 # skip if job1 failed
  job3:
    needs: [job1, job2]
```
