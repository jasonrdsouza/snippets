# Git Spells

## Move master branch pointer to previous commit
For example, if you accidentally commit to master instead of making a branch
```
git reset --hard master~1
```

## Remove unnecessary whitespace

http://git-scm.com/docs/git-stripspace

```
git stripspace
```

## See unique authors

```
git log | grep "Author" | sort | less | uniq -c
```

## Create an archive of the code (ignoring gitignored files!)

```
git archive --format zip --output <filepath> master
```

You can replace `master` in the command above with and tag, branch, or sha

## Bailing out of an in-progress merge

```
git merge --abort
```
