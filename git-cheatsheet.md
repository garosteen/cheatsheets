# GIT CHEATSHEET

## Basic Workflow ##

### Initializing Repository ###

* `git init` - Initialize the current directory into a git repo.
* `git clone <URL>` - Clone an existing repository into a directory named after the repository
  * `git clone <URL> <directory>` - Clone into a different directory

### Adding files ###

* `git add <file>` - Add file to staging area
* `git add -A`
* `git add .` -  Add all untracked files

### Committing ###

* `git commit` - Commit
  * `-m "message"` - Add commit message
  * `-a` - Commit all changes to tracked files (does not add new files)
  * `--amend` - Alter last commit message

### Pushing ###

* `git remote add origin <URL>`
* `git push -u origin master`
  * `-u` - Set GitHub as upstream repository (download changes automatically with pull).

### Branches ###

* `git branch` - View current branches
  * `-a` - View all branches (including those associated with remote origin)
* `git checkout <branch>` - Check out a branch
  * `-b` - Create new branch
  * `-d` - Delete branch (if merged)
  * `-D` - Delete branch (even if unmerged)

## Getting Information ##

* `git status`
* `git log`
  * `--oneline` - Keep it to one line per commit
  * `--graph` - Show a little graph on the side
  
* `git diff` - Show diff between last commit and unstaged changes in current project.
  * `--staged` - Show diff between last commit and staged changes.
* `git show <SHA>`
* `git remote -v` - Show URL of remote branch

## Initial Configurations ##

* `git config --global user.name "Your Name"` - Set global name variable
* `git config --global user.email your.email@example.com` - Set global email variable

## Miscellaneous Commands ##

* `$ git remote set-url origin git@github.com:User/project-name.git` - Change origin URL
* `git config --global alias.name-of-alias "command to run"` - Set a git alias
  * e.g. `git config --global alias.graph "log --graph --oneline --decorate"`
