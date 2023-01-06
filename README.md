# Sway-arch dotfiles
Everything you/I need to know about my EndeavourOS + Hyprland setup.

# Currently still in progress, please star this for later [I'll be done by end-March, have exams to tackle]

# WARNINGS/DEPENDENCIES: 
- `qt5ct`, `qt6-wayland`, `qt5-wayland`
- I have `udiskie &` and `lxpolkit &` in startup, under `# Startup Apps` in `hyprland.conf`. `lxpolkit` is for authentication so that my file manager can get authorization for mounting my external HDD. (*Install `lxsession` if you want `/usr/bin/lxpolkit`, as `lxpolkit` is not a package as such.*) Please remove this line if you want.
- This doesn't work for any pulseaudio-related packages, I've completely switched to `pipewire` and `wireplumber` (wpctl)
- `playerctl` for media controls
- Currently, `yay` custom build directory does not work, so manually add it in `~/.config/yay/config.json` see this: https://github.com/Jguer/yay/issues/1612

# Useful stuff

- For viewing removable drives with file managers, install `gvfs`
- Install `lxappearance` for GTK/icon configuration, *TIP: Widget style means gtk theme.* 
- For GTK3/4 set environment variable `GTK_THEME=theme_name` and GTK2 use `GTK_RC_FILES`
- Setup `udiskie`: https://github.com/coldfix/udiskie/wiki/Usage
-`lxpolkit`: https://wiki.archlinux.org/title/Polkit#Authentication_agents
- Waybar icons not working (fresh install): https://github.com/Alexays/Waybar/issues/117
- XWayland and blurry issues: https://github.com/hyprwm/Hyprland/pull/591
- ^^^^ for electron: https://wiki.archlinux.org/title/wayland#Electron

- *hyprland docs are SUPREME.*
> https://wiki.hyprland.org/Getting-Started/Quick-start/ | 
> https://wiki.hyprland.org/Configuring/Variables/ | 
> https://wiki.hyprland.org/Configuring/Configuring-Hyprland/ | 
> https://wiki.hyprland.org/Useful-Utilities/ | 
> https://github.com/hyprwm/Hyprland/wiki/FAQ | 
> https://wiki.hyprland.org/Configuring/Monitors/ (global display scale)


- *wofi*:
> https://hg.sr.ht/~scoopta/wofi | https://man.archlinux.org/man/wofi.1.en
