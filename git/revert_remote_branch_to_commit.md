# Reverting Git Remote Branch to Commit Older than the most recent commit

There will come a time when a remote branch needs to be reverted to an old branch beyond the last commit. Use the code below to choose a commit to revert to and create a branch to PR against the master/main branch

```
git checkout -f remote_branch -- .
git checkout -B new_branch
git commit -a
git push origin new_branch
```

Open a new PR against your main/master branch and merge to revert.
