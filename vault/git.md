---
id: q6pJclRsTZxkELPEhZmaM
title: Git
desc: ''
updated: 1630332614750
created: 1629355098634
---

Roll back to previous commit

    git checkout -b old xxxxxx
    git reset --hard xxxxxx # beware!

Revert the initial commit:

    git update-ref -d HEAD # Update the object name stored in a ref safely, delete HEAD

Turn off paged output:

    git config --global pager.branch false

## Clean up

list merged branches:

    git branch --merged origin/main
