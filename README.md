# Hyprland and KDE config files from Jens
## Hyprland
![Screenshot](https://raw.githubusercontent.com/JensDeLeersnyderPXL/arch-dotfiles/main/screenshots/hyprland_screenshot.png)

## KDE 
![Screenshot](https://raw.githubusercontent.com/JensDeLeersnyderPXL/arch-dotfiles/main/screenshots/KDE_screenshot.png)

## Install
### Yay

Run as user NOT ROOT!
```
git clone https://aur.archlinux.org/yay-bin
cd yay-bin
makepkg -si
```

### Packages
```
yay -S hyperland-bin sddm-git kitty waybar-hyprland vim tldr nano micro brave-bin dolphin vscode json-c curl cmake python-pip libappindicator-gtk3 github-desktop-bin onlyoffice-bin
```

## Configuration Sddm
```
Session=Hyprland.desktop
User=Jens
Numlock=true
```

## Install nerd font
```
mkdir -p $HOME/Downloads```/nerdfonts/
cd $HOME/Downloads/"
wget https://githubcom/ranoasis/nerd-fonts/releases/download/v2.3.1/CascadiaCode.zip
unzip '*.zip' -d $HOME/Downloads/nerdfonts/
rm -rf *.zip
sudo cp -R $HOME/Downloads/nerdfonts/ /usr/share/fonts/
```
## Waybar Weather
### Install python module
```
pip install requests
```
## Install nvidia drivers
```
yay -S nvidia
```
# KDE-Plasma
## install KDE
```
yay -S plsama kde-network-meta kde-system-meta kde-utilities-meta plasma-wayland-session
```
- Global Theme used: [Utterly Sweet](https://store.kde.org/p/1906500)
- SDDM   Theme used: [Sweet](https://github.com/EliverLara/Sweet/tree/nova/kde/sddm)
- Package   Updates: [Command Output](https://store.kde.org/p/1166510/)

## KDE restore/backup tools
- [transfuse](https://gitlab.com/cscs/transfuse)
### Backup
```
./transfuse.sh -b CURRENTUSER
```
### Restore
```
./transfuse.sh -r PATIENT
```
## Sources used making these

- Official Hyprland Github <https://github.com/hyprwm/Hyprland>
- Linux Mobiles Hyprland dot files <https://github.com/linuxmobile/hyprland-dots>
- Christitus Start <https://github.com/ChrisTitusTech/hyprland-titus>
