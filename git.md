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

## Create an archive of the code (ignoring gitignored files!)

```
git archive --format zip --output <filepath> master
```

You can replace `master` in the command above with and tag, branch, or sha
