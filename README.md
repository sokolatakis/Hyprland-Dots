<div align="center">

# 💌 ** My fork of JaKooLit's Hyprland Dot Files ** 💌

<br/>
</div>

## 👁️‍🗨️ My Hyprland install Scripts 👁️‍🗨️
- You can install Hyprland using JaKooLit's Scripts below:

- [Fedora-Linux](https://github.com/JaKooLit/Fedora-Hyprland)

- [Debian/Ubuntu-Linux](https://github.com/JaKooLit/Debian-Hyprland)

- [Arch-Linux](https://github.com/JaKooLit/Arch-Hyprland)

## ✨ Copying instructions. 
- Note! The auto copy script will create backups of intended folders to be copied. However, still a good idea to manually backup just incase script failed to backup!

- ~/.config (btop cava dunst gtk-3.0 hypr kitty rofi swappy swaylock waybar wlogout) - These are folders to be copied.
- ~/Pictures/wallpapers - Will be backed up

### 🔔 Automatic copy of configurations
> clone this repo by using git. Change directory, make executable and run the script
```bash
git clone https://github.com/JaKooLit/Hyprland-Dots.git
cd Hyprland-Dots
chmod +x copy.sh
./copy.sh
```
### 🐌 Manual copy (not recommended for newbies)
- Backup your existing folders in ~/.config (advisable)
- copy all contents of configs into ~/.config, overwriting all
- copy contents of wallpapers into ~/Pictures/wallpapers/ (create wallpapers folder if required)
- make the Hyprland scripts executable 
```bash
chmod +x $HOME/.config/hypr/scripts/*
```
- Make sure to execute initial symlinks else dunst, wofi and waybar will fail to launch
```bash
ln -sf "$HOME/.config/waybar/configs/config-default" "$HOME/.config/waybar/config"
ln -sf "$HOME/.config/waybar/style/style-pywal.css" "$HOME/.config/waybar/style.css"
ln -sf "$HOME/.config/dunst/styles/dunstrc-dark" "$HOME/.config/dunst/dunstrc"
```
- after that initialize pywal with
```wal -i wallpaper/path```
- then run this 
```bash
ln -sf "$HOME/.cache/wal/colors-rofi-dark.rasi" "$HOME/.config/rofi/pywal-color/pywal-theme.rasi"
```
- Before reboot or logout, choose wallpaper with SUPER CTRL W.
### All credits go to [JaKooLit](https://github.com/JaKooLit) and his cool rices
