# GIT CHEATSHEET

## Basic Workflow

### Initializing Repository

    $ git init
    
    $ git status

### Adding files

    $ git add <file>
    $ git add -A
        Add all untracked files.
    $ git add .
        Same effect, adds the current directory

### Committing ###

    $ git commit -m "message"
        -a
            commit all changes to existing files (but does not add new files)
        --amend
            Alter last commit message

### Pushing ###

    $ git remote add origin <URL>
    $ git push -u origin master
        -u
            sets GitHub as upstream repository (download changes automatically with pull)


## Getting Information

    $ git status
    $ git log
    $ git diff
        shows diff between last commit and unstaged changes in current project.
        --staged
            Show diff between last commit and staged changes
    $ git show <SHA>

## Initial Configurations

    $ git config --global user.name "Your Name"
    $ git config --global user.email your.email@example.com

## Miscellaneous Commands

    Change origin URL:
        $ git remote set-url origin git@github.com:User/project-name.git

------------------------------------------------------------
git add -A
    Add all files or directories to staging area

git add <name>


