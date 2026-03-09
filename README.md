# wally
Wayland wallpaper picker built with bash, rofi & awww.

<img width="1920" height="1080" alt="wally_screenshot" src="https://github.com/user-attachments/assets/2efd1c5e-06fb-4733-a060-96fa8c949647" />

### Setup
1. Create an environment variable that points to the local wallpaper directory. Be sure to adjust the path as necessary to reflect your local system.
```bash
export WALLPAPER_HOME="${HOME}/Pictures/Wallpapers" 
```
2. Follow instructions for awww installation below. 
```bash
https://codeberg.org/LGFae/awww
```
3. Install the remaining prerequisites using your system's package manager.
```bash
sudo pacman -S bash rofi
```
4. Clone the repository to a local directory and create a link in XDG_BIN_HOME so your local user will have access.
```bash
git clone git@github.com:Dayguy/wally.git ~/Projects/
cd ~/Projects/wally
ln -s ./wally ${HOME}/.local/bin/wally 
```
5. You can create a keybind to Windows + W or any other key combination by adding the following to hyprland.conf or other configuration. Be sure to adjust for your system.
```bash
bind = $mainMod, W, exec, uwsm-app -- wally
```
### Final Thoughts
That should be it! You can launch wally via the key bind or by entering wally o the command line.

