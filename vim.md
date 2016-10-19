# Vim Spells

## Spacing

### Convert tabs to spaces
*assumes `expandtab` is on*

```
:retab
```

### Strip trailing whitespace
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
<LEADER>-<hjkl>
```

Open a split with a specific file
```
:sp filename
:vsp filename
```

## Scratch space

- courtesy of https://github.com/mtth/scratch.vim plugin
- `gs` in normal mode opens the scratch window and enters insert mode. The scratch window closes when you leave insert mode.
= can also use `:Scratch`

## Uppercase a word
```
gUiw
```

## Execute command on multiple lines

The `g` command is the "global" command to execute other commands. In this case, you can use it with the `norm` command to perform a change on lines that match a specific pattern (or all lines).

For example, if you want to add a semicolon to the end of all lines that start with a number, you could do that as follows:
```
:g/^\d/norm A;
```
In this case, instead of substituting the line for something else, you are telling Vim to execute the "normal mode" command of moving to the end of the line and entering insert mode (with `A`), and then adding a semicolon.

This is pretty powerful because you have the ability to perform a motion on all the lines matching a specific pattern.

## Visual select and insert

```
CTRL-v
```

Once you have selected the block you want, you can edit all of the selected lines at once with:

```
SHIFT-i (insert whatever you want) <ESC>
```


