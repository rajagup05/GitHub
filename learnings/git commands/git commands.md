## 1. git config user.name "your name" 

=> The command `git config user.name "your name"` sets the username for Git commits, either for a specific repository or globally for all your repositories. 

[ sets username for the current local git repo to track who made the commits in this repo. ]

**For all your repositories (global setting):**


git config --global user.name "Your Name") sets the username for all Git repositories on your system.

git add -> add files to staging area and stores all the changes in .git folder

git log -> it tells what was changed , when and who has made that changes.

git diff -> it is similar to git status but advanced version of it. It can show what has been added, removed, etc. between working dir and staging env or changes between two commits or staged but non commited messages or unstaged changes or diff between two branches.

Whenever you commit any changes a unique commit id/hash is generated.
Git is a version control tool which tracks every changes made.

git revert commit id/hash -> it is used to revert the changes made/pushed to remote github repo.

git reset HEAD~1 -> it uncommits the file/recent changes from staging area.

git restore --staged filename -> unstage the file/changes.

git clean -> The git clean command in Git is used to remove untracked files from the working directory. Untracked files are those that exist in your local repository but are not currently being managed by Git (i.e., they haven't been added to the staging area with git add or committed). 

