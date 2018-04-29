# GIT CHEATSHEET

## Basic Workflow

### Initializing Repository

`$ git init`

### Adding files

`$ git add <file>`

`$ git add -A`

Add all untracked files.

`$ git add .`

Same effect; add the current directory

### Committing ###

Command|Description
----|----
`$ git commit`|Commit
`-m "message"`|Add commit message
`-a`|Commit all changes to tracked files (does not add new files)

`$ git commit -m "message"`

`-a`

Commit all changes to existing files (but does not add new files)

`--amend`

Alter last commit message

### Pushing ###

`$ git remote add origin <URL>`

`$ git push -u origin master`

`-u`

Set GitHub as upstream repository (download changes automatically with pull).


## Getting Information

`$ git status`

`$ git log`

`$ git diff`

Show diff between last commit and unstaged changes in current project.

`--staged`

Show diff between last commit and staged changes.

`$ git show <SHA>`

## Initial Configurations

`$ git config --global user.name "Your Name"`

`$ git config --global user.email your.email@example.com`

## Miscellaneous Commands

Change origin URL:
`$ git remote set-url origin git@github.com:User/project-name.git`
