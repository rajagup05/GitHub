## git reset

**Modes of `git reset`:**

The three main modes determine what happens to your files after moving the branch pointer. 

- `--soft`:  
  - Moves the branch HEAD pointer to the specified commit. \
  - Keeps changes staged in the index and untouched in the working directory. \
  - Use case: Reorganize or combine multiple commits into a single, cleaner one, ready for immediate recommit.


- `--mixed (Default)`:
  - Moves the branch HEAD pointer to the specified commit.
  - Unstages the changes from the index, but leaves them as modified files in the working directory.
  - Use case: Undo commits and the staging process, allowing you to re-evaluate and selectively stage the changes again from scratch. You can run git status to see the changes as "not staged for commit".
