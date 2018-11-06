## Global CONFIG


```
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

## Alias

To: add > commit > pull > push
```
git config --global alias.call '!func(){ git add . && git commit -aqm "$1" && git pull origin $2 -q --no-progress && git push origin $2 -q ; }; func
```
Usage: `$ git call 'First commit' master`

## ignore chmod
`git config core.fileMode false`

