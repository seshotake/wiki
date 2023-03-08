# bat

An alternative to `cat` command

## Fatures:

- syntax highlighting
- git integration
- show non-printable chracters
- automatic paging for large files
- file concatenation

Install `bat` in Arch Linux:

```sh
sudo pacman -S exa
```

### Concate two files to one

```sh
bat file1 file2 > target_file
```

### Append content to file to another

```sh
bat path/to/file >> target_file
```

### Show numbers on all lines

```sh
bat --number path/to/file
```

### Use as a colorizing pager for `man`

Add to your `.bashrc`:

```bash
export MANPAGER="sh -c 'col -bx | bat -l man -p'"
```
