# Dev Environment Setup

This is a collection of settings, references, and config files for software development on MacOS

## Things to Install

### Terminal Toys

```bash
brew install cowsay
brew install fortune
```

### Fonts

```bash
brew tap homebrew/cask-fonts
brew install --cask font-fira-code
brew install --cask font-hack-nerd-font
brew install --cask font-cascadia-code
brew install --cask font-cascadia-code-pl
brew install --cask font-cascadia-mono
brew install --cask font-cascadia-mono-pl
```

### ZSH Stuff

- homebrew
- ohmyzsh
- zsh-syntax-highlighting
- zsh-autosuggestions
- powerlevel10k

### Setup Powerlevel 10k

run `p10k configure`

### Apps

- VS Code
- VS Code Insiders
- Cleanshot (paid replacement for mac screenshots)
- Karabiner (`caps lock` -> `esc`)
- Apptivate (`⌃` + `⌘ `+ `t` -> open iTerm2)
- Rectangle
- AltTab (windows-style alt-tab for MacOS - change default `⌥` to `⌘`)
- Raycast (free replacement for spotlight and alfred - set to `⌘` + `space`)

## VS Code Setup

- .zshrc
- settings.json (vs code settings `/Users/$USER/Library/Application Support/Code/User/settings.json`)

### Generate Extension Install Commands

Run this on original machine to backup extension list
This will generate a file to run on the new machine

```bash
code --list-extensions | xargs -L 1 echo code --install-extension >> install_vsc_exts.sh
```

or just generate a list with `code --list-extensions >> vsc_ext_list`

### Bulk Install Extensions

Run this on new machine once VS Code is installed

```bash
sh ./install_vsc_exts.sh
```
# config_macos
