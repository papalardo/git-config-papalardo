# Git cmds

### Alias 
**git call 'Description commit' master/branch** 
> For to: add > commit > pull > push
```
git config --global alias.call '!func(){ git add . && git commit -aqm "$1" && git pull origin $2 -q --no-progress && git push origin $2 -q ; }; func
```

### ignore chmod
> git config core.fileMode false

### remove ignored files
```
git ls-files --ignored --exclude-standard -z | xargs -0 git rm --cached
git commit -am "Remove ignored files" 

git update-index --assume-unchanged .env
git update-index --no-assume-unchanged .env
```
