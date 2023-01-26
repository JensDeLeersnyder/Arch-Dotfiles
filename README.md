# Hyprland config files from Titus

![Screenshot](https://github.com/ChrisTitusTech/hyprland-titus/raw/main/hyprland-titus.png)

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
yay -S hyperland-bin sddm-git kitty waybar-hyprland vim tldr nano micro brave-bin dolphin vscode json-c curl cmake python-pip libappindicator-gtk3
```

## configuration sddm
Session=Hyprland.desktop
User=Jens
Numlock=true

## install nerd font
mkdir -p $HOME/Downloads/nerdfonts/
cd $HOME/Downloads/
wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.3.1/CascadiaCode.zip
unzip '*.zip' -d $HOME/Downloads/nerdfonts/
rm -rf *.zip
sudo cp -R $HOME/Downloads/nerdfonts/ /usr/share/fonts/

# waybar weather
## install python module
pip install requests

## Gotchas

- Recommend archinstall with Sway as desktop for base
- SDDM-GIT is required or you will run into shutdown bugs and delays
- SDDM needs to be configured for autologin (recommend using swaylock on start of script for security)

## Bugs

- Hyprland is still in beta (0.2) as of the creation of these dot files
- Sometimes my RX5700XT goes to sleep and requires a reload, because it is stuck on black screen.

## Work In Progress

- [ ] Help Popup with Hotkey
- [ ] Wayland guide for nwg-look, wlr-randr, etc.
- [ ] Synergy Workaround - Looking at waynergy or just using KVM
- [ ] Gamescope Addition - Adding more parity with Steamdeck features
- [ ] More Customizations for Waybar - Battery, Backlight, etc.
- [ ] Auto-configuration - Long term goal

## Sources used making these

- Official Hyprland Github <https://github.com/hyprwm/Hyprland>
- Linux Mobiles Hyprland dot files <https://github.com/linuxmobile/hyprland-dots>
