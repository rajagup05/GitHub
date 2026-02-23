
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

#### 1. **Cookies (Browser-Based State):** 

Cookies are small pieces of data stored on the client side (your browser) that are automatically sent back to the server with every request. 

- **Role in GitHub:** Primarily used for browser-based user interaction. When you log in to GitHub via your browser, a `user_session` cookie is set, allowing you to browse, comment, and commit without re-entering your password.
- **Key Security Flags:** GitHub uses `Secure` (sent only over HTTPS) and `HttpOnly` (inaccessible to JavaScript) flags to prevent session hijacking and Cross-Site Scripting (XSS) attacks.
- **DevOps Example:** If you are using the GitHub web interface to manage pull requests, your session is maintained by cookies.

#### 2. Sessions (Server-Side State)

A session is a server-side storage object that keeps track of user data during their visit. The session is usually identified by a unique, random string called a Session ID, which is stored in a cookie on the client side. 

- Role in GitHub: When you log in, GitHub generates a session in their database and gives your browser a user_session cookie containing the ID. This allows them to know which user is making a specific request to github.com.
- Expiration: Sessions are temporary. If you are inactive for a long time, GitHub will delete the session on the server side, making the cookie on your browser useless, and you will be logged out. 
