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
```sh
$ git commit -a -m "message here"
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
$ git checkout -b <feature-name>
```

Create an orphan branch
```sh
$ git checkout --orphan gh-pages
```

###Merge Branches
Merge feature branch into master
```sh
$ git merge <feature-branch>
```

###Remove Branches
Delete a local branch
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

Remove all changes to a file since last commit
```sh
$ git checkout -- <file name>
```
