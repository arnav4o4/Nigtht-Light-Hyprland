## Night Light Feature in Hyprland

When using **Gnome** or **KDE** , we use **Night light** option present in settings:

**KDE**
![KDE Plasma 5.17: Thunderbolt, X11 Night Color and Redesigned Settings - KDE  Community](https://kde.org/announcements/plasma/5/5.17.0/night-color.png)


**GNOME**

![Night Light Slider - GNOME Shell Extensions](https://extensions.gnome.org/extension-data/screenshots/screenshot_1276_gNya1IO.png)

Alternative to these there are some software like Redshift that can be used..

## But in Hyprland, apps like Redshift doesn't support.

<a href="https://ibb.co/18sdt3S"><img src="https://i.ibb.co/Gcst4Xh/image.png" alt="image" border="0"></a>

Source: [Redshift -Arch](https://wiki.archlinux.org/title/redshift)

So there is a **configuration tool** called [Hyprshade](https://github.com/loqusion/hyprshade)

**Screenshots:**
**Vibrance**![Vibrance](https://github.com/loqusion/hyprshade/raw/main/.github/assets/vibrance.png)

**Blue light filter**
![Blue Light Filter](https://github.com/loqusion/hyprshade/raw/main/.github/assets/blue-light-filter.png)

To install [AUR- Hyprland](https://aur.archlinux.org/packages/hyprshade) on Arch :

    yay -S hyprshade

the command `blue light shader` is the one use to change the screen color temperature.

    hyprshade on blue-light-filter
in case you want to increase the color `/usr/share/hyprshade/examples/config.toml` is where you can change the value

If you want to use hyprshade command by using buttons , u can add keybindings in the `.config/hypr/keybindings.conf` file

for example

    bind  = $mainMod, F9, exec, hyprshade on blue-light-filter
    bind  = $mainMod, F7, exec, hyprshade on vibrance

And done!!  Now you can use night light feature on **hyprland**
