# dotfiles-hyprland
Everything you/I need to know about my EndeavourOS + Hyprland setup.

# WARNINGS: 
- I have `udiskie` in startup, under `# Startup Apps` in `hyprland.conf`. I use this for automount a couple of removable drives. Please remove this line if you want.
- This doesn't work for any pulseaudio-related packages, I've completely switched to `pipewire` and `wireplumber` (wpctl)

# Useful stuff

- Arch is hard so I used endeavourOS
> run `sudo pacman -Sy archlinux-keyring' first in the installation .iso before running the calamares installer

- For viewing removable drives with file managers, install `gvfs`
- Setup `udiskie` if you want automount https://github.com/coldfix/udiskie/wiki/Usage
- Waybar icons not working (fresh install): https://github.com/Alexays/Waybar/issues/117
- Volume inc/dec with `wireplumber` + `pipewire` + `pipewire-pulse`
```
wpctl set-volume @DEFAULT_AUDIO_SINK@ [num%]+-
```

- *hyprland docs are SUPREME.*
> https://wiki.hyprland.org/Getting-Started/Quick-start/ | 
> https://wiki.hyprland.org/Configuring/Variables/ | 
> https://wiki.hyprland.org/Configuring/Configuring-Hyprland/ | 
> https://wiki.hyprland.org/Useful-Utilities/ | 
> https://github.com/hyprwm/Hyprland/wiki/FAQ

- gettin scaling to work (XWayland)
> https://wayland.freedesktop.org/xserver.html

- *wofi*:
> https://hg.sr.ht/~scoopta/wofi | https://man.archlinux.org/man/wofi.1.en
