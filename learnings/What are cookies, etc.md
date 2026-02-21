
**git remote add origin <remote_repository_URL>**

> The `git remote add origin` command adds a new remote repository to your local Git repository and names it "origin". This allows you to push and pull changes between your local project and a shared remote server like GitHub, GitLab, or Bitbucket. 

The general syntax for the command is:
`git remote add <name> <url>`

By convention, the name origin is used for the primary remote repository. You should replace `<url>` with the actual HTTPS or SSH URL provided by your hosting service. 

Example: `git remote add origin https://github.com/username/your-repo.git`

### Typical Workflow

This command is typically used after you have initialized a local repository and made your first commit: 

1. **Initialize Git in your project directory**: `git init`.
2. **Add and commit your files**:
    `git add ..`
    `git commit -m "Initial commit"`.
3. **Add the remote repository (use the URL from your hosting service)**: `git remote add origin <repository-url>`.
4. **Verify the remote was added**: `git remote -v`.
5. **Push your local commits to the remote**: `git push -u origin main` (or master depending on your branch name). The `-u` flag sets the upstream branch so future git push and git pull commands don't require specifying the remote and branch names. 



### What are cookies, tokens, sessions?
