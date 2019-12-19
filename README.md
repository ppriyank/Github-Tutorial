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


