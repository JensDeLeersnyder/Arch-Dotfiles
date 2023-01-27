# Hyprland and KDE config files from Jens
## Hyprland
![Screenshot](https://raw.githubusercontent.com/JensDeLeersnyderPXL/arch-dotfiles/main/hyprland_screenshot.png)

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

## Configuration sddm
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
## waybar weather
### Install python module
```
pip install requests
```
## Install nvidia drivers
```
yay -S nvidia
```
## Install kde
```
yay -S plsama kde-applications plasma-wayland-session
```
- Global Theme used: [Utterly Sweet](https://store.kde.org/p/1906500)
- SDDM   Theme used: [Sweet](https://github.com/EliverLara/Sweet/tree/nova/kde/sddm)
- Package   Updates: [Command Output](https://store.kde.org/p/1166510/)
## Sources used making these

- Official Hyprland Github <https://github.com/hyprwm/Hyprland>
- Linux Mobiles Hyprland dot files <https://github.com/linuxmobile/hyprland-dots>
