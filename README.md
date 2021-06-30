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

### Reseting file changes 
```
git checkout filename
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
```
*.DS_Store*
dist/*
target/
lib_managed/
src_managed/
/.idea/
__pycache__
*.class
```

### Deleting a file only from a repository
```
git rm file2.txt /path/to/the/file --cached
git rm folder/* --dry-run
```
doing just `rm` deletes the files from file system as well

### disable username/password based git push

The git is cloned via https, change it to ssh: 
```
git remote set-url origin git@github.com:username/repo.git
```

### Changing last commit message
```
git commit --amend
```
