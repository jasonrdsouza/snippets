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

## See unique authors (by commit amount)

```
git shortlog -sn

# Optionally specifying start and end date
git shortlog -sn --since='10 weeks' --until='2 weeks'
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

## Ignore whitespace in diff

```
git diff -w
git show -w
```

## Show changed words instead of lines

```
git diff --word-diff
```

## Apply a patch
Most often, the "patch" will be a diff file created with `git diff`.

```
git checkout <BRANCH_TO_APPLY_PATCH_TO>
git apply <PATH_TO_PATCH_FILE>
```
