# recreating branch earlier deleted

After force delete of the branch `git --delete --force <branch>` or `git -D <branch>`
and trying to create the same branch in local repository by `git checkout <branch>` 
you can occur an error: `error: pathspec <branch> did not match any file(s) known to git`
To recreate the branch use command: `git checkout -b <branch>` 
Your branch will be recreated in local git repository.

---
_Last update: 28 February 2023_