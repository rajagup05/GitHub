
### git revert

The `git revert` command is used to undo the changes of a specific commit by creating a new commit that contains the exact opposite changes. Unlike `git reset`, it does not delete or alter the project's history, making it the safest way to undo changes in shared or public repositories. 

### Commands: 

- Revert the latest commit: `git revert HEAD`
- Revert a specific commit: `git revert <commit-hash>`

### Key Differences: Revert vs. Reset: 

- `git revert`: \
  Preserves history; adds a new commit \
  Safe for shared/public branches \
  New commit is created

- `git reset`: \
  Rewrites history; removes commits \
  Best for local, unpushed changes \
  Branch pointer is moved back



  
