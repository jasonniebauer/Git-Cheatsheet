Git Tips
========

###Global Configuration
```git
$ git config --global user.name "GitHub username"
$ git config --global user.email "GitHub email address"
$ git config --global color.ui true
$ git config --global core.excludesfile ~/.gitignore_global
```

###Help
```git
$ git help <command>
```

###Add files to staging area
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

Remove a file that is being tracked
```git
$ git rm <file>
```
