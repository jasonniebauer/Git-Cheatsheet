Git Tips
========

###Global Configuration
```sh
$ git config --global user.name "GitHub username"
$ git config --global user.email "GitHub email address"
$ git config --global color.ui true
$ git config --global core.excludesfile ~/.gitignore_global
```

Add Files to Ignore
```sh
$ nano ~/.gitignore_global
```

###Help
```sh
$ git help <command>
```

###Initialization
Initialize Git Repository in Directory
```sh
$ git init
```

###Show Remote Repositories
```sh
$ git remote -v
```

###Adding a Remote Repository
```sh
$ git remote add <name> <address>
```
Example
```sh
$ git remote add origin <Github repo url>
```

###Remove a Remote Repository
```sh
$ git remote rm <name>
```

###Push to Remote
Origin: remote repository name, master: local branch to push
```sh
$ git push -u <name> <branch>
```
Example
```sh
$ git push -u origin master
```

###Clone a Repository
```sh
$ git clone <repository-url>
```

###Clone Repository and Rename
```sh
$ git clone <repository-url> <new-name>
```

###Status
```sh
$ git status
```

###Add Files to Staging Area
Add the list of files
```sh
$ git add <list of files>
```

Add all files
```sh
$ git add -a
```

Add all txt files in current directory
```sh
$ git add *.txt
```

Add all txt files in sepcific directory
```sh
$ git add /docs*.txt
```

Add all files in specific directory
```sh
$ git add /docs*
```

Add all txt files in the whole project
```sh
$ git add "*.txt"
```

###Skip Staging Area and Commit
Add changes from all tracked files
```sh
$ git commit -a -m "commit message"
```

###Remove Files
Remove a file that is being tracked
```sh
$ git rm <file>
```

###Commit Files
Commit all staged files
```sh
$ git commit m "your message here"
```

###Undoing a Commit
Undo last commit, put changes into staging
(HEAD^ means move to the last commit before 'HEAD')
```sh
$ git reset --soft HEAD^
```
Undo last commit and all changes
```sh
$ git reset --hard HEAD^
```
Under last two commits and all changes
```sh
$ git reset --hard HEAD^^
```

###Adding to a Commit
Add another file or change to the previous commit and override commit message
```sh
$ git commit --amend -m "new commit message"
```

###Push Files to Repository
Push files to master branch
```sh
$ git push
```

Push files to another branch
```sh
$ git push origin <branch-name>
```

###Create Branches
Create a feature branch
```sh
$ git branch <feature-name>
```

Create a feature branch and check it out
```sh
$ git checkout -b <feature-name>
```

Create an orphan branch
```sh
$ git checkout --orphan gh-pages
```

Link Local Branch to the Remote Branch
```sh
$ git push origin <branch-name>
```

###Check which Branch you are on
```sh
$ git branch
```

###List all Remote Branches
```sh
$ git branch -r
```

###Remote Show
Shows remote branches and whether they are tracked or not, local branches and which branches they merge with, and local branches configured for git push and whether they are out of date or not.
```sh
$ git remote show <remote-name>
```

###Switching to a Branch
```sh
$ git checkout <branch-name>
```

###Check the Git Log
```sh
$ git log
```

###Merge Branches
Merge feature branch into master
```sh
$ git merge <feature-branch>
```

###Remove Branches
Delete a local branch (clean up)
```sh
$ git branch -d <branch-name>
```

Remove a remote branch (*Use Caution*)
```sh
$ git push origin :<branch-name>
```

###Viewing Unstaged Differences
View unstaged differences since last commit
```sh
$ git diff
```

###Viewing Staged Differences
View staged differences since last commit
```sh
$ git diff --staged
```

###Discard Changes
Unstage a file (head refers to last commit)
```sh
$ git reset HEAD <file name>
```

Remove all changes to a file since the last commit
```sh
$ git checkout -- <file name>
```

###Remove all changes to multiple files in the last commit
Chain files together in a single command
```sh
$ git checkout -- <file 1 name> <file 2 name>
```
