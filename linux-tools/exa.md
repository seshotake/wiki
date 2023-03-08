# exa

An alternative to `ls` command

## Features:

- uses colors for file types and metadata
- knows about symlinks, extended attributes, and git
- queries files in parallel
- built-in `tree` tool
- column view support

Install `exa` in Arch Linux:

```sh
sudo pacman -S exa
```

### List files one per line

```sh
exa --oneline
```

### List all files, including hidden

```sh
exa -a
```

### Long format list (permissions, ownership, size and midification date) of all files:

```sh
exa -al
```

### Don't list files mentioned in `.gitignore`

```sh
exa --git-ignore
```
