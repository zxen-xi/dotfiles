# Hyprland + Arch dotfiles
Everything you/I need to know about my EndeavourOS + Hyprland setup.

# Currently still in progress, please star this for later [I'll be done by end-March, have exams to tackle]

Waybar gradient borders (credit [flick0](https://github.com/flick0) on Hyprland discord)
```css
#workspaces button.active label{
    color: #fff;
    font-weight: bolder;
    padding-left: 17px;
    padding-right: 17px;
    border-radius: 15px;
    background-color: #000;
}

#workspaces button.active{
    padding-right: 3px;
    box-shadow: rgba(0, 0, 0, 0.288) 2 2 5 2px;
    padding-left: 3px;
    padding-bottom: 3px;
    background: rgb(203,166,247);
    background: radial-gradient(circle, rgba(203,166,247,1) 0%, rgba(193,168,247,1) 12%, rgba(249,226,175,1) 19%, rgba(189,169,247,1) 20%, rgba(182,171,247,1) 24%, rgba(198,255,194,1) 36%, rgba(177,172,247,1) 37%, rgba(170,173,248,1) 48%, rgba(255,255,255,1) 52%, rgba(166,174,248,1) 52%, rgba(160,175,248,1) 59%, rgba(148,226,213,1) 66%, rgba(155,176,248,1) 67%, rgba(152,177,248,1) 68%, rgba(205,214,244,1) 77%, rgba(148,178,249,1) 78%, rgba(144,179,250,1) 82%, rgba(180,190,254,1) 83%, rgba(141,179,250,1) 90%, rgba(137,180,250,1) 100%); 
    background-size: 400% 400%;
    animation: gradient_f 10s ease-in-out infinite;
    transition: all 0.3s cubic-bezier(.55,-0.68,.48,1.682);
}
```

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
