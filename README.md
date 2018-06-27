# git-config-papalardo

[ alias ] 
add > commit > pull > push
git config --global alias.call '!func(){ git add . && git commit -aqm "$1" && git pull origin master -q --no-progress && git push origin master -q ; }; func'

[ ignore chmod ]
git config core.fileMode false
