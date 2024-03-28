# Oh My Posh themes

A collection of personal themes to be used with Oh My ZSH / Oh My Posh

## Prerequisites

###  Install Oh My ZSH!

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Add the following configuration to `.zshrc`:

```shell
# Path to your oh-my-zsh installation.
export ZSH="$HOME/.oh-my-zsh"
plugins=(macos brew z git sudo poetry aliases colored-man-pages)  # These are personal preferences
source $(brew --prefix)/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
source $(brew --prefix)/share/zsh-autosuggestions/zsh-autosuggestions.zsh
source $ZSH/oh-my-zsh.sh
```

###  Install Oh My Posh

```shell
brew install jandedobbeleer/oh-my-posh/oh-my-posh
```

Add the following configuration to `.zshrc`:

```shell
# Oh My Posh -- edit your preferred theme
if [ "$TERM_PROGRAM" != "Apple_Terminal" ]; then
  eval "$(oh-my-posh init zsh --config $(brew --prefix oh-my-posh)/themes/chosenone-blues.omp.json)"
fi
```

### Install fonts

```shell
brew tap homebrew/cask-fonts  # you only need this once
brew search nerd-font         # Search for font packages
brew install --cask font-meslo-lg-nerd-font 
```

### Install iTerm2

```shell
brew install --cask iterm2
```

Add the following configuration to `.zshrc`:
```shell
# iTerm2 integration
export ITERM2_SQUELCH_MARK=1
source ~/.iterm2_shell_integration.zsh
```

## Themes

### Chosen One - [Blues](themes/chosenone-blues.omp.json)

![Chosen One - Blues](images/blues.png)

### Chosen One - [Collab](themes/chosenone-collab.json)

![Chosen One - Collab](images/collab.png)

### Chosen One - [Easter](themes/chosenone-easter.omp.json)

![Chosen One - Tonbal](images/easter.png)

### Chosen One - [Jicor](themes/chosenone-jicor.omp.json)

![Chosen One - Tonbal](images/jicor.png)

