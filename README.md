# Quickstart

## Install fresh

```bash
# Install fresh
bash <(curl -sL https://get.freshshell.com)

$(echo export FRESH_RCFILE=$HOME/.dotfiles/.freshrc) >> .zshrc
```

## Install dotfiles
### Quick install using env var
```bash
# Set GitHub user/org
GH_DOTFILES_USER=beecorrea

# Quick install with fresh environment var
FRESH_LOCAL_SOURCE='${GH_DOTFILES_USER}/dotfiles' \
  bash -c <(curl -sL https://get.freshshell.com)
```


### Manual install
```bash
# Set GitHub user/org
GH_DOTFILES_USER=beecorrea

# Clone repo
git clone 'git@github.com:${GH_DOTFILES_USER}/dotfiles.git' ~/.dotfiles

export FRESH_RCFILE="$HOME/.dotfiles/.freshrc"

# Install dotfiles
fresh install
```

