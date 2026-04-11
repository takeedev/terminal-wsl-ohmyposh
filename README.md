# terminal-wsl-ohmyposh
setting terminal

## Install WSL
```shell
wsl --install
```

## Open WSL
```shell
sudo apt update
sudo apt install zsh git curl fzf unzip -y
```

## Change shell to zsh 
```shell
chsh -s $(which zsh)
```

## Install Oh-My-Posh 
```shell
curl -s https://ohmyposh.dev/install.sh | bash -s
```

## set oh-my-posh
```shell
vim ~/.zshrc
export PATH="$HOME/.local/bin:$PATH"
eval "$(oh-my-posh init zsh --config 'https://raw.githubusercontent.com/JanDeDobbeleer/oh-my-posh/main/themes/M365Princess.omp.json')"
source ~/.zshrc
oh-my-posh --version
```

## Install highlighting 
```shell
sudo apt install zsh-autosuggestions zsh-syntax-highlighting
# autosuggest
source /usr/share/zsh-autosuggestions/zsh-autosuggestions.zsh
# syntax highlight
source /usr/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
# fzf
[ -f ~/.fzf.zsh ] && source ~/.fzf.zsh
```

## Install mise en place 
```shell
curl https://mise.run | sh
echo 'eval "$(~/.local/bin/mise activate zsh)"' >> ~/.zshrc
source ~/.zshrc
mise --version
```
