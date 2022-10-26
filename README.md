
# MyMacBox



## Install Brew

The Missing Package Manager for macOS
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Run these three commands in your terminal to add Homebrew to your PATH:
```
echo '# Set PATH, MANPATH, etc., for Homebrew.' >> /Users/grenaud/.zprofile
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/grenaud/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## Install packages

### iTerm2
```brew install --cask iterm2```

### Ohmyzsh
```sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"```


```
brew install --cask homebrew/cask-fonts/font-meslo-for-powerline
brew install font-powerline-symbols
```

### Google Chrome
```brew install google-chrome```

### Visual Studio Code
```brew install --cask visual-studio-code```

### Microsoft Teams
```brew install microsoft-teams```

### KeePassXC
```brew install --cask keepassxc```

### Screenshot with Flameshot
```brew install flameshot```

### Hashicorp tools
```brew install terraform```



## Config
### SSH Key Gen

ecdsa - a new Digital Signature Algorithm standarized by the US government, using elliptic curves. This is probably a good algorithm for current applications. Only three key sizes are supported: 256, 384, and 521 (sic!) bits. We would recommend always using it with 521 bits, since the keys are still small and probably more secure than the smaller keys (even though they should be safe as well). Most SSH clients now support this algorithm.
```ssh-keygen -t ecdsa -b 521```
