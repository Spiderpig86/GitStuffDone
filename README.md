# GitStuffDone
Simple git reference for when I forget.

## Creating Repositories
* `git init` - create a new repo
* `git clone <repo url> <folder name>` - download a project to a custom folder
* `git status` - check repo status

## Repo Logging
* `git log` - display commit ID (SHA), author, date, and commit message
* `j`(up), `k`(down), `q`(exit) - scrolling through commit history
* `git log --stat` - view modified files
* `git log -p` or `git diff` - view file changes in commit
* `git log -p --stat` - view both modified files and file chanegs
* `git show <SHA id>` - view file changes of specific SHA id
* `git show SHAid --state` - view modified files of specific SHA
* `git log --stat <SHA id>` - view specific commit by ID
