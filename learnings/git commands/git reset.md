## git reset

**Modes of `git reset`:**

The three main modes determine what happens to your files after moving the branch pointer. 

- `--soft`:  
  - Moves the branch `HEAD` pointer to the specified commit. \
  - **Keeps** changes staged in the index and untouched in the working directory. \
  - **Use case**: Reorganize or combine multiple commits into a single, cleaner one, ready for immediate recommit.


- `--mixed (**Default**)`:
  - Moves the branch HEAD pointer to the specified commit.
  - **Unstages** the changes from the index, but leaves them as modified files in the working directory.
  - **Use case**: Undo commits and the staging process, allowing you to re-evaluate and selectively stage the changes again from scratch. You can run `git status` to see the changes as "not staged for commit".

- `--hard`:
  - Moves the branch `HEAD` pointer to the specified commit.
  - **Discards** all changes in both the staging area and the working directory.
  - **Use case**: Completely abandon all recent work (committed and uncommitted) and revert to a clean slate of a previous commit. This is a destructive action and should be used with extreme caution on local branches only, as the changes may be permanently lost. 


**Common git reset Commands:**

  - **Unstaging a file**: To unstage a specific file while keeping local changes, use git reset <file> or the equivalent git restore --staged <file>.
  - **Undoing the last commit but keeping the changes**: Use git reset --soft HEAD~1.
  - **Completely discarding recent commits and changes**: Use the destructive command git reset --hard HEAD~1 to move back one commit and remove all subsequent changes.
  - **Discarding all local uncommitted changes**: Use git reset --hard HEAD to revert the working directory and index to the last committed state. 
