# ccd

customiezd cd

## Features

- change directory from selected by fzf
- do not change basic cd behavior
- cd to specific subdirs
- allow file path
- accept stdin
- cd to parent directories
- cd to histories directories

## Usage

```
ccd /path/to/dir/.                select from subdirs
ccd /path/to/dir/..               select from subdirs (recursive)
ccd /path/to/dir/file             cd to /path/to/dir
find /path/to/dir/ -type d | ccd  select from stdin
ccd ...                           select from parent directories
ccd --                            select from histories
```

## Configuration

$CCD_FINDER set fuzzy finder (default fzf).

## Installation

```
$ curl -sS https://raw.githubusercontent.com/yosugi/ccd.zsh/master/ccd.zsh > ~/.ccd.zsh
$ echo '[ -f ~/.ccd.zsh ] && source ~/.ccd.zsh && setopt AUTO_PUSHD' >> ~/.zshrc
$ exec $SHELL -l
```

## License

MIT License

## Version

0.1.0
