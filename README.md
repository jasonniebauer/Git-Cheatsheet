Git Tips
========

###Global Configuration
```git
$ git config --global user.name "GitHub username"
$ git config --global user.email "GitHub email address"
$ git config --global color.ui true
$ git config --global core.excludesfile ~/.gitignore_global
```

###Add Files to Ignore
```git
$ nano ~/.gitignore_global
```

###Help
```git
$ git help <command>
```

###Status
```git
$ git status
```

###Add Files to Staging Area
Add the list of files
```git
$ git add <list of files>
```

Add all files
```git
$ git add -a
```

Add all txt files in current directory
```git
$ git add *.txt
```

Add all txt files in sepcific directory
```git
$ git add /docs*.txt
```

Add all files in specific directory
```git
$ git add /docs*
```

Add all txt files in the whole project
```git
$ git add "*.txt"
```

###Remove Files
Remove a file that is being tracked
```git
$ git rm <file>
```

###Commit Files
Commit all staged files
```git
$ git commit m "your message here"
```

###Push Files to Repository
Push files to master branch
```git
$ git push
```

Push files to another branch
```git
$ git push origin gh-pages
```

###Create a Branch
Create a feature branch
```git
$ git checkout -b <feature-name>
```

Create a gh-pages branch
```git
checkout --orphan gh-pages
```

###Merge Branches
Merge feature branch into master
```git
$ git merge <feature-branch>
```
