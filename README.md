# devenv-config

## Installation for NVIM Config
### Ubuntu
#### Install 

##### Install Nerd Font
```
sudo wget -P /usr/local/share/fonts https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf
sudo wget -P /usr/local/share/fonts https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf
sudo wget -P /usr/local/share/fonts https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf
sudo wget -P /usr/local/share/fonts https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf
```

Update font-cache
```
fc-cache -fv
```
Verify Installation
```
fc-list | grep Meslo
/usr/local/share/fonts/MesloLGS NF Bold.ttf: MesloLGS NF:style=Bold
/usr/local/share/fonts/MesloLGS NF Bold Italic.ttf: MesloLGS NF:style=Bold Italic
/usr/local/share/fonts/MesloLGS NF Regular.ttf: MesloLGS NF:style=Regular
/usr/local/share/fonts/MesloLGS NF Italic.ttf: MesloLGS NF:style=Italic
```

Note: Reboot system after this to take effect

##### Install Neovim
```
sudo apt-get install neovim
```

##### Install Ripgrep
```
sudo apt-get install ripgrep
```

##### Install Nodejs
```
sudo apt-get install nodejs
```
##### Install Lazygit
```
LAZYGIT_VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | grep -Po '"tag_name": "v\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/latest/download/lazygit_${LAZYGIT_VERSION}_Linux_x86_64.tar.gz"
tar xf lazygit.tar.gz lazygit
sudo install lazygit /usr/local/bin
```

#### Setup Config
copy the neovim folder to .config in $HOME directory
