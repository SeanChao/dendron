---
id: vLN66cbj18kIA9aNMw4MV
title: GitHub Actions
desc: ''
updated: 1636544252506
created: 1629255661366
---

Github actions snippets.

[Syntax reference](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions)

```yml
on:
  schedule:
    - cron: '0 20 */3 * *' # Runs at 20:00 UTC every 3 days.

on:
  push:
    branches:
      - main
      - dev

jobs:
  job1:
  job2:
    needs: job1 # skip if job1 failed
  job3:
    needs: [job1, job2]
    runs-on: ubuntu-latest
    steps:
      - uses: ncipollo/release-action@v1
        with:
          allowUpdates: true
          artifacts: "target/release/file"
          token: ${{ secrets.GITHUB_TOKEN }}
      - name: Deploy 🚀
        uses: JamesIves/github-pages-deploy-action@4.1.5
        with:
          branch: gh-pages # The branch the action should deploy to.
          folder: build # The folder the action should deploy.
```
