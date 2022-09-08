# Branching
## Rename a branch

```
git branch -m <oldname> <newname>
```

# Stashing
## Named stashes
Save a stash with a name
```
git stash push -m "stash-name"
```

This will add a message at the end of the stash so you can easily find which stash you want to apply

List stashes
```
git stash list
```

Apply/pop stashes
```bash
# Create a stash with a given name
git stash -m "my-stash"

# List stashes
git stash list

# look for your stash:
# stash@{0}: On dev/merging-manager-modules-components-project-groups-licenses: my-stash

# Pop by index
git stash pop stash@{0}
```

# Recovery
## Recover a deleted branch/commit
- [How to Restore a Deleted Branch or Commit with Git Reflog](https://rewind.com/blog/how-to-restore-deleted-branch-commit-git-reflog/)