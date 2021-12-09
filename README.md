# ua4iugi-dev
dev

# git
- setup
```
$ git clone https://github.com/nilcy/ua4iugi-dev.git
$ cd ua4iugi-dev
$ git flow init -d
$ git add .; git commit -m "UP2DATE"; git push
```
- develop
```
$ git branch
$ git status
$ git add .; git commit -m "UP2DATE"; git push
```
- release
```
$ tag=`date +%Y%m%d-%H%M%S`
$ git flow release start $tag
$ git log --oneline --decorate=short > CHANGELOG.md
$ git add .; git commit -m "UP2DATE"; git push
$ git flow release finish $tag
$ git push origin --all
```