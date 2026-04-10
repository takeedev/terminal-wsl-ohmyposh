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
