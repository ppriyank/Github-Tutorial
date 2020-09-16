# Github-Tutorial

### Compare File between 2 commits 
```
git log  # commit id for 2 commits 
git commit_id1 commit_id2 -- file
```

### Pushing deleted file on github
```
git rm <file-name>
```
### Reseting a file to a particular commit 
```
git checkout <commit_ID> path/to/the/file.txt
```

### Deleting last n commits 
```
git reset HEAD~n
```
to reflefct the **deleted commit on remote**: 
```
git push --force
```

### Stashing changing before pull
```
git stash
git pull 
git stash clear 
```


### Adding files to .gitignore 
```
git config --global core.excludesfile '~/.gitignore'
echo '.ipynb_checkpoints' >> ~/.gitignore
```

### Deleting a file only from a repository
```
git rm file2.txt /path/to/the/file --cached
git rm folder/* --dry-run
```
doing just `rm` deletes the files from file system as well

