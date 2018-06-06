# My Site Open Source

## Commands to alter remotes

### See remotes
```PowerShell
git remote -v
```

### Defaults

https://meuappopensource.visualstudio.com/MyApp/_git/MySite (fetch)
https://meuappopensource.visualstudio.com/MyApp/_git/MySite (push)

### Target

https://meuappopensource.visualstudio.com/MyApp/_git/MySite (fetch)
https://github.com/tiagopariz/MySite.git (push)

### Create branch
```PowerShell
git checkout master
git pull
git checkout -b tiago-change-anything```

### Edit the files

(...)

### Send to repository

```PowerShell
git status
git add --all
git commit --message "Description"
git push
```

### Open the Pull request

tiago-change-anything --> develop
develop --> master

### Send to GitHub
```PowerShell
git checkout master
git pull
git remote set-url --add --push origin https://github.com/tiagopariz/MySite.git
git push
```

### Restore to defaulr
```PowerShell
git remote set-url --delete --push origin https://github.com/tiagopariz/MySite.git
git remote set-url --add --push origin https://meuappopensource.visualstudio.com/MyApp/_git/MySite
```