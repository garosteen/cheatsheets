# GIT CHEATSHEET

## Basic Workflow

### Initializing Repository

Command|Description
-------|-----------
`git init`|Initialize the current directory into a git repo.

### Adding files

Command|Description
-------|-----------
`git add <file>`|Add file to staging area
`git add -A`
`git add .`| Add all untracked files

### Committing ###

Command|Description
-------|-----------
`git commit`|Commit
`-m "message"`|Add commit message
`-a`|Commit all changes to tracked files (does not add new files)
`--amend`| Alter last commit message

### Pushing ###

Command|Description
-------|-----------
`git remote add origin <URL>`|
`git push -u origin master`|
`-u`|Set GitHub as upstream repository (download changes automatically with pull).


## Getting Information

Command|Description
-------|-----------
`git status`|
`git log`|
`git diff`|Show diff between last commit and unstaged changes in current project.
`--staged`|Show diff between last commit and staged changes.
`git show <SHA>`|

## Initial Configurations

Command|Description
-------|-----------
`git config --global user.name "Your Name"`|Set global name variable
`git config --global user.email your.email@example.com`|Set global email variable

## Miscellaneous Commands

Command|Description
-------|-----------
`$ git remote set-url origin git@github.com:User/project-name.git`|Change origin URL
