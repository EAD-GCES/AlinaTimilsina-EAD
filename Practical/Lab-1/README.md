## Setting up a new repository
Git is a content management and tracking system developed by Linus Torvalds, creator of Linux. It includes a directory that continuously changes as codes are added throughout application or website development. Git also tracks revisions that are performed on stored data.

### Setup and init
1. Create a new repo in github.
2. Create a new local directory to contain the project.
3. Open Terminal.
4. Change the current working directory to our local project.
5. Configuring user information used across all local repositories <br>
```git config --global user.name “[firstname lastname]”```
set a name that is identifiable for credit when review version history
`git config --global user.email “[valid-email]”`
set an email address that will be associated with each history marker
6. Initialize the local directory as a Git repository.
   `git init [project directory]`
7. Retrieve an entire repository from a hosted location via URL
   `git clone [url]`

8. Create a README.md file
   `touch README.md`
9. Show modified files in working directory, staged for your next commit
 `git status`
10. Add the files in your new local repository. This stages them for the first commit.
    `git add .`
    To only add a file
    `git add [filename]` 
11. Commit the files that you've staged in your local repository.
    `git commit -m "[First commit]"`
12. In Terminal, add the URL for the remote repository where your local repository will be pushed.
    `git remote add origin  [REMOTE_URL]`
13. Push the changes in your local repository.
    `git push -u origin master`

### Branching, Merging
Create new branch
`git branch [branch name]`
Deleting a branch 
`git branch -d [branch name]`
for force delete 
`git branch -D [branch name]`
Switch to different branch
`git checkout [branch name]`
Add a git URL as an alias
`git remote add [alias] [url]`
Fetch down all the branches from that Git remote
`git fetch [alias]`
Merge branch
`git merge [alias]/[branch]`

### Fetching

Fetch changes from the remote, but not update tracking branches.
   `git fetch [remote]`
Fetch from specified branch
    `git fetch [remote] [branch]`
Fetch all remotes and their branches
    `git fetch --all`
Fetch changes from the remote and merge current branch with its
upstream.
` git pull [remote]`
Push local branch to remote repository. Set its copy as an upstream.
`git push -u [remote] [branch]`