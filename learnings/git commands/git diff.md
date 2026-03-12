
## git diff 

=> it is similar to `git status` but advanced version of it. It can show what has been added, removed, etc. between working dir and staging env or changes between two commits or staged but non commited messages or unstaged changes or diff between two branches.

The `git diff` command is a fundamental Git utility used to display the differences between various states of a repository, such as between the working directory and the staging area, two commits, or two branches. It helps developers review and understand changes in their codebase in a standardized format. 

### Common `git diff` Usages:

1. `git diff` (**View unstaged changes**): This shows changes in your working directory that you have not yet added to the staging area with `git add`.

2. **View staged changes**: These commands display the differences between the staging area (index) and the last commit (`HEAD`), allowing you to review exactly what will be included in the next commit.


`git diff --staged`
#### or
`git diff --cached`

3. `git diff HEAD`: Shows all local changes (both staged and unstaged) compared to the most recent commit. (Working Directory vs. Last Commit)

4. `git diff <commit1> <commit2>`: Compares the snapshots of two different commits. (Two specific commits)

5. `git diff <branch1> <branch2>`: Compares the tips of two different branches.

6. `git diff <file_path>`:  Shows changes in a specific file in the working directory compared to the staging area. 
