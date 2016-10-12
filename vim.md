# Vim Spells

## Convert tabs to spaces

*assumes `expandtab` is on*

```
:retab
```

## Strip trailing whitespace

```
:%s/\s\+$//e
```

## Splits

Creating them
```
:sp (horizontal split)
:vsp (vertical split)
```

Jumping around them
```
CTRL-<hjkl> (movement keys)
```

## Scratch space

courtesy of https://github.com/mtth/scratch.vim plugin

`gs` in normal mode opens the scratch window and enters insert mode. The scratch window closes when you leave insert mode.


