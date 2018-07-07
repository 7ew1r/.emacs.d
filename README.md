# Emacs

GNU Emacs 25.3.1

## Requirements
- [Cask](https://github.com/cask/cask)
- [Pandoc](https://pandoc.org)
- [cmigemo](https://github.com/koron/cmigemo)

## Installation

### 1. Clone repo

``` shell
$ git clone https://github.com/RTewi/.emacs.d.git
```
### 2. Make symbolic-link

``` shell
$ ln -sfv /path/to/repo/.emacs.d $HOME
```

### 3. Cask

``` shell
$ brew install cask # Homebrew
or
$ curl -fsSL https://raw.githubusercontent.com/cask/cask/master/go | python
```

Add the following to .bashrc (or .zshrc)

``` shell
export PATH="$HOME/.cask/bin:$PATH"
```

```
$ source ~/.bashrc
```

``` shell
$ cask upgrade
$ cd ~/.emacs.d
$ cask
```

### 4. 3rd-party

``` shell
$ brew install pandoc cmigemo llvm # Homebrew
or
$ sudo apt install pandoc cmigemo llvm-dev clang libclang-dev cmake # Ubuntu
```

### 5. codic

Get codic API token from [codic](https://codic.jp/)

``` shell
$ mkdir ~/.emacs.d/spec
$ vi ~/.emacs.d/spec/codic-api-token
"codic-api-token"
```
