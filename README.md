
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


## Config
### SSH Key Gen

From https://www.ssh.com/academy/ssh/keygen page : 

ecdsa - a new Digital Signature Algorithm standarized by the US government, using elliptic curves. This is probably a good algorithm for current applications. Only three key sizes are supported: 256, 384, and 521 (sic!) bits. We would recommend always using it with 521 bits, since the keys are still small and probably more secure than the smaller keys (even though they should be safe as well). Most SSH clients now support this algorithm.
```ssh-keygen -t ecdsa -b 521```


### Upgrade Python

Upgrade pip
```python3 -m pip install --upgrade pip```

### Install Ansible

Install Ansible via pip
```pip3 install ansible```
```ansible-galaxy collection install community.general```

### Install with Ansible all Brew packages
Run the playbook in order to install all brew packages
```ansible-playbook playbook.yml```


## Configure Shell

### Ohmyzsh
Oh My Zsh is a delightful, open source, community-driven framework for managing your Zsh configuration. It comes bundled with thousands of helpful functions, helpers, plugins, themes, and a few things that make you shout...
```sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"```

### ZSH config gile
Update your bin path to $PATH in your .zsrhc file like : 
```export PATH=$HOME/bin:/usr/local/bin:$PATH:/Users/$USER/Library/Python/3.9/bin```

Update to your favorite ZSH_THEME, on my side agnoster
```ZSH_THEME="agnoster"```

And other params like 
```
ENABLE_CORRECTION="true"
COMPLETION_WAITING_DOTS="true"
````

