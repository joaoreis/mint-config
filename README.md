# Mint-config
My config files and setup instructions for new Linux Mint installs

### Snap
`sudo apt install snap`

### Remmina - Remote Desktop Client
```
sudo apt-add-repository ppa:remmina-ppa-team/remmina-next
sudo apt update
sudo apt install remmina remmina-plugin-rdp remmina-plugin-secret remmina-plugin-spice
```
### Git 
```
sudo apt install git
snap install gitkraken
```
### Android Studio configs and plugins
```
sudo apt-get install qemu-kvm libvirt-bin ubuntu-vm-builder bridge-utils ia32-libs-multiarch
sudo adduser $USER kvm
sudo chown $USER /dev/kvm
```

### Some Snap programs
```
snap install slack
snap install spotify
```

### Other programs

### Oh My ZSH
```sudo apt install zsh
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```

Set ZSH_THEME=powerlevel10k/powerlevel10k in your ~/.zshrc.

Download the fonts:


[MesloLGS NF Regular.ttf](https://github.com/romkatv/dotfiles-public/raw/master/.local/share/fonts/NerdFonts/MesloLGS%20NF%20Regular.ttf)

[MesloLGS NF Regular.ttf](https://github.com/romkatv/dotfiles-public/raw/master/.local/share/fonts/NerdFonts/MesloLGS%20NF%20Bold.ttf)

[MesloLGS NF Regular.ttf](https://github.com/romkatv/dotfiles-public/raw/master/.local/share/fonts/NerdFonts/MesloLGS%20NF%20Italic.ttf)

[MesloLGS NF Regular.ttf](https://github.com/romkatv/dotfiles-public/raw/master/.local/share/fonts/NerdFonts/MesloLGS%20NF%20Bold%20Italic.ttf)


```
sudo apt install libglib2.0-bin
gsettings set org.gnome.desktop.interface monospace-font-name 'MesloLGS NF 11'
```

#### Sublime Text
```
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
sudo apt install apt-transport-https
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt update
sudo apt install sublime-text
```
