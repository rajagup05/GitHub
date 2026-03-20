## git reset

**Modes of `git reset`:**

The three main modes determine what happens to your files after moving the branch pointer. 

1. `--soft`:  

Moves the branch HEAD pointer to the specified commit. \
Keeps changes staged in the index and untouched in the working directory. \
Use case: Reorganize or combine multiple commits into a single, cleaner one, ready for immediate recommit.
