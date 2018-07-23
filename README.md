# git-config-papalardo

### alias 
add > commit > pull > push
> git config --global alias.call '!func(){ git add . && git commit -aqm "$1" && git pull origin master -q --no-progress && git push origin master -q ; }; func'

### ignore chmod
> git config core.fileMode false

### remove ignored files
> git ls-files --ignored --exclude-standard -z | xargs -0 git rm --cached
> git commit -am "Remove ignored files"
git commit -am "Remove ignored files"
