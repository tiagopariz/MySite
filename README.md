# My Site Open Source

## Commands to alter remotes

### See remotes
`git remote -v`

### Defaults

https://meuappopensource.visualstudio.com/MyApp/_git/MySite (fetch)
https://meuappopensource.visualstudio.com/MyApp/_git/MySite (push)

### Target

https://meuappopensource.visualstudio.com/MyApp/_git/MySite (fetch)
https://github.com/tiagopariz/MySite.git (push)

### Create branch
`git checkout master`
`git pull`
`git checkout -b tiago-change-anything`

### Edit the files

(...)

### Send to repository

`git status`
`git add --all`
`git commit --message "Description"`
`git push`

### Open the Pull request

tiago-change-anything --> develop
develop --> master

### Send to GitHub
`git checkout master`
`git pull`
`git remote set-url --add --push origin https://github.com/tiagopariz/MySite.git`
`git push`

### Restore to defaulr
`git remote set-url --delete --push origin https://github.com/tiagopariz/MySite.git`
`git remote set-url --add --push origin https://meuappopensource.visualstudio.com/MyApp/_git/MySite`