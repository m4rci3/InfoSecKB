### Make a directory a Git repository 

```bash
git init . 
#Turns the current working directory into a Git repository
```

### Make specific files to be ignored 

```bash
vim {or nano} .gitignore
# Place this in the branch's repo, all you need to do is list the file's name in the file. 
```

### See what files have been modified, added or deleted since the last commit.

```bash
git status
```

### Create , list, delete  branches: 

```bash
git branch
```

### Switch to a different branch in the repository 

```bash
git checkout {branchname}
```

### See the logs of any commits:

```bash
git log 
```

### Show difference between the current state of your files and the last commit. Helps to see changes

```bash
git diff
```

### Stage changes for commit. Telling Git to include your modified or new files in the next commit. Adding your changes to a list of updates you want to save permanently

```bash
git add {name of modified file}

#For a specific file that you want to update 
git add .# makes changes to all of the files within the branch 
#git stage is an alias for the above commands
```

### Unstage / unadd  

```bash
git restore --staged {file} 
# Or . (representing the current working directory/branch)
```

### Delete a *local* branch
```bash
git branch -d <branch>
# Only deletes the branch if it has already been fully merged in its upstream branch 

git branch -D <branch> 
# Alias for --delete --force, which deletes the branch irrespective of its merged states 
```

### Delete a remote branch
```bash
git push -d <remote name> <branch name>
```


### Commit the changes

```bash
git commit -m "Short summary here, becomes the commits title" -m "More detailed explanation of the changes. This section gives greater clarity for those reading the history of the repo. Adds to the body of the commit message. "


```

### Push the changes made to the GitHub repository: 

```bash
git push 
```

