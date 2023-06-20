# Arch-Linux

# Installation
1. Download the iso from the official website https://archlinux.org/download/.
2. Install it in a virtual machine
3. `pacman -Sy archinstall archlinux-keyring`
4. `archinstall`
5. Tweak settings from the menu
6. Click on **Install** or Save your config for future use.
7. `reboot`

# Desktop Environment
1. `sudo pacman -Sy git vim`
2. `mkdir -p ~/.local/gits/`    
3. `cd ~/.local/gits/`
4. `git clone https://github.com/bugswriter/dwm.git` 
5. `git clone https://github.com/bugswriter/dmenu.git`
6. `git clone https://github.com/bugswriter/st.git`
7. Go to each directory and `sudo make clean install`
8. Install the dependencies it is asking for `sudo pacman -Sy <..whatever..>`
9. `cp /etc/X11/xinit/xinitrc ~/.xinitrc`
10. `vim ~/.xinitrc`
11. Delete everything below **twm...**.
12. Add `exec dwm` there.
13. `sudo pacman -S ttf-jetbrains-mono ttf-font-awesome`

These are bugswriter's keybindings:
![Key Bindings](https://github.com/harshdeepcodes/Arch-Linux/assets/94488766/5953279c-bbd0-44b2-9fe3-e75433b41e2d)

# Customizationss
## For setting zsh as default shell
```bash
chsh -s $(which zsh)
```

## For setting the resolution
```bash
sudo pacman -Sy xorg-xrandr
xrandr --output Virtual-1 --mode 1920x1080
```

## For Wallpaper and Pywal Setup
```bash
sudo pacman -Sy xwallpaper python-pywal <..anybrowser..>
xwallpaper -zoom <..wallpaper..>
```
