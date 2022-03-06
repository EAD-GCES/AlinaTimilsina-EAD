## Setting up a new repository
Git is a content management and tracking system developed by Linus Torvalds, creator of Linux. It includes a directory that continuously changes as codes are added throughout application or website development. Git also tracks revisions that are performed on stored data.

### Setup and init
1. Create a new repo in github.
2. Create a new local directory to contain the project.
3. Open Terminal.
4. Change the current working directory to our local project.
5. Configuring user information used across all local repositories <br>
```{git config --global user.name “[firstname lastname]”}```<br>
set a name that is identifiable for credit when review version history<br>
`git config --global user.email “[valid-email]”`<br>
set an email address that will be associated with each history marker<br>
6. Initialize the local directory as a Git repository.<br>
   `git init [project directory]`
7. Retrieve an entire repository from a hosted location via URL<br>
   `git clone [url]`

8. Create a README.md file<br>
   `touch README.md`
9. Show modified files in working directory, staged for your next commit<br>
 `git status`
10. Add the files in your new local repository. This stages them for the first commit.<br>
    `git add .`<br>
    To only add a file<br>
    `git add [filename]` <br>
11. Commit the files that you've staged in your local repository.<br>
    `git commit -m "[First commit]"`
12. In Terminal, add the URL for the remote repository where your local repository will be pushed.<br>
    `git remote add origin  [REMOTE_URL]`<br>
13. Push the changes in your local repository.<br>
    `git push -u origin master`

### Branching, Merging
Create new branch<br>
`git branch [branch name]`<br>
Deleting a branch <br>
`git branch -d [branch name]`<br>
for force delete <br>
`git branch -D [branch name]`<br>
Switch to different branch<br>
`git checkout [branch name]`<br>
Add a git URL as an alias<br>
`git remote add [alias] [url]`<br>
Fetch down all the branches from that Git remote<br>
`git fetch [alias]`<br>
Merge branch<br>
`git merge [alias]/[branch]`<br>

### Fetching

Fetch changes from the remote, but not update tracking branches.<br>
   `git fetch [remote]`<br>
Fetch from specified branch<br>
    `git fetch [remote] [branch]`<br>
Fetch all remotes and their branches<br>
    `git fetch --all`<br>
Fetch changes from the remote and merge current branch with its
upstream.<br>
` git pull [remote]`<br>
Push local branch to remote repository. Set its copy as an upstream.<br>
`git push -u [remote] [branch]`