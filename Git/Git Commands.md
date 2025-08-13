### Make a directory a Git repository

```bash
git init . 
#Turns the current working directory into a Git repository
```


### Make specific files to be ignored

```bash
vim {or nano} .gitignore
# place this in the branches repo, all you need to do is list the filename in the file.
```

### See what files have been modified, added or deleted since the last commit

```bash
git status
```

### What to do after you rename a file

```bash
git rm {old file name}
# After the renaming of a file there will be an untracked file (the new name of the file that was renamed) and a file that was "deleted"(the name of the old file), in order to properly continue you NEED to make these changes before continuing. 
```

### Create , list, delete branches

```bash
git branch
```

### Switch to a different branch in the repository

```bash
- [x] git checkout {branchname}
```

### See the logs of any commits

```bash
git log 
```

### Show difference between the current state of your files and the last commit. Helps to see changes

```bash
git diff
```

### Stage changes for commit. It tells Git to include your modified or new files in the next commit. Adding your changes to a list of updates you want to save permanently

```bash
git add {name of modified file} # for a specific file that you want to update 
git add .# makes changes to all of the files within the branch 
```

### Unstage

```bash
git restore --staged {file}
```

### Delete a LOCAL branch

```bash
git branch -d <branch> 
#Only deletes the branch if it has already been fully merged in its upstream branch.
git branch -D <branch> 
#Alias for --delete --force, which deletes the branch "irrespective of its merged status"
```

### Delete a remote branch

```bash
git push -d <remote name> <branch name>
```

### Commit the changes

```bash
git commit -m "Short summary here, becoming the commit's title" -m "More detailed explanation of the changes. This section gives greater clarity for those reading the history of the repo. Adds to the body of the commit message. "
```

### Push the changes made to the GitHub repository

```bash
git push 
```

### Set & Check git identity

```bash
#Set your git username and email globally meaning you only do this once, otherwise \
#if you have already run it but want to override this setting you can set this inside \
#the current working repository that you wish to change it in \
#These will be "immutably baked into the commits you start creating" 
git config user.name "git acc username"
git config user.mail "git acc email" 

#You can view all of your settings and where they are coming from using \
#this will also show the path where it is saved to.
git config --list --show-origin
```

