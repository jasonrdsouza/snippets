# Git Spells

## Remove unnecessary whitespace

http://git-scm.com/docs/git-stripspace

```
git stripspace
```

## See unique authors

```
git log | grep "Author" | sort | less | uniq -c
```
