# GitStuffDone
Simple git reference for when I forget.

## Creating Repositories
* `git init` - create a new repo
* `git clone <repo url> <folder name>` - download a project to a custom folder
* `git status` - check repo status

## Repo History
* `git log` - display commit ID (SHA), author, date, and commit message
* `j`(up), `k`(down), `q`(exit) - scrolling through commit history
* `git log --stat` - view modified files
* `git log -p` or `git diff` - view file changes in commit
* `git log -p --stat` - view both modified files and file chanegs
* `git show <SHA id>` - view file changes of specific SHA id
* `git show SHAid --state` - view modified files of specific SHA
* `git log --stat <SHA id>` - view specific commit by ID
* 
## Adding
* `git add .` - add all files in current directory to stage
* `git add <file names with space as delimiter>` - add specific files to stage
* `git add -u` - add all tracked files

## Committing
* `git commit -m <message>` - write a commit message without using the text editor
    * Guideline: https://udacity.github.io/git-styleguide/
* `git commit` - write commit message with text editor opened
* `git commit -a` - directly add files to the repo without going through staging

## GitIgnore
* Note: Assumes that VSCode is installed.
##### Linux / OSX / GitBash
1. Run `touch .gitignore` to create a file
2. Run `code .gitignore` to open and edit

##### Windows Powershell
1. Run `New-Item .gitignore -type file` to create a file
2. Run `code .gitignore` to open and edit

##### Windows CMD
1. Run `copy NUL .gitignore` to create a file
2. Run `code .gitignore` to open and edit

## Tagging
* `git tag` - check version of tag in command line
* `git tag -a <tag name>` - write a message for a specific version of the file
* `git log --decorate` - show the current branch and tag version
* `git tag -d <tag name> - delete tag version
* `git tag -a <tag name> <SHA id>` - add a tag for a specific commit by SHA id.

## Branching
* `git branch` - show current branch
* `git branch <branch name>` - create a new branch
* `git checkout <existing branch name>` - switch to another branch
* `git log --oneline --decorate` - display current active branch with SHA id and commits only
* `git branch -d <branch name>` - delete branch by name
* `git checkout -b <branch name>` - create new branch and switch to it
* `git checkout -b <branch name> master` - create a new branch in the same location as the master branch and switch to it
* `git log --oneline --decorate --graph --all` - display all branches in folder

## Merging
* `git reset --hard HEAD^` - undo branch merge
* `git merge <branch name>` - merge branch by name

## Correcting
* `git commit --amend` - correct commit details in branch
