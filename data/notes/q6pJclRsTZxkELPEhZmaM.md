
Revert local changes:

    git checkout .
    git clean -fd # force, and recursive into dirs

Roll back to previous commit

    git checkout -b old xxxxxx
    git reset --hard xxxxxx # beware!

Revert local modifications to a file:

    git checkout HEAD -- <file>

Revert the initial commit:

    git update-ref -d HEAD # Update the object name stored in a ref safely, delete HEAD

Turn off paged output:

    git config --global pager.branch false

Squash and merge:

    git merge --squash bugfix

## Clean up

list merged branches:

    git branch --merged origin/main
