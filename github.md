# Github Spells

## Ignore Whitespace in Diff

Add `?w=1` to the URL to see the diff with whitespace ignored

## Plaintext Patch and Diff view

- Add `.diff` to a pull request (or individual commit) url to get a plaintext diff view
- Likewise, add `.patch` to get a plaintext patch view

## Adjust Tab Space in view

Add `?ts=4` to the URL to change the width of tab characters to 4 spaces

## Gist embedded view mode

Add `.pibb` to the end of a Gist url in order to get an HTML only version of the gist suitable for display

## Line highlighting

Adding `#L52` to the end of a code file url will highlight that line. Clicking the line works as well.
This also works with ranges, like `#L53-L60`. Holding shift and clicking the two lines works as well.

## Closing issues via Commit Messages

If a particular commit fixes an issue, any of the keywords `fix/fixes/fixed`, `close/closes/closed`
or `resolve/resolves/resolved`, followed by the issue number, will close the issue once it is committed
to the master branch.

## Public SSH Keys

You can get a list of public ssh keys in plain text format by visiting:

```
https://github.com/{user}.keys
```

