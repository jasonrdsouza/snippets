# Process Substitution


Creating a named pipe is done in [fish](https://fishshell.com/) with the `psub` command as follows:

```
diff (sort a.txt | psub) (sort b.txt | psub)
```

References: `man psub`
