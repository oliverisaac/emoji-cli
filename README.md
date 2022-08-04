# emoji: output emojis on the cli

Of note: the actual script doesn't really do much, but it is an excellent example of how you can write tools that chain other tools together to make your life easier.

## Usage:

Each command line argument will search for an emoji.

For example:

**Search first for apple, then for peach:**
```bash
emoji apple peach
```` 

**Search for apple fruit as a single emoji:**
```bash
emoji "apple fruit"
```

## Use it in your git commit:

```bash
git commit -a -m "$( emoji rocket ): bumping version to v1"
```

## Installation:

This CLI requires two tools: `emoji-fzf` and `fzf`:

- [emoji-fzf](https://github.com/noahp/emoji-fzf): `pip install emoji-fzf`

- [fzf](https://github.com/junegunn/fzf): `brew install fzf`
