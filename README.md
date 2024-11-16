# Adwaita-colors

![showcase](./v2.3.1.jpg)

Adwaita Colors enhances the Adwaita icon theme by integrating GNOME’s accent color feature, introduced in GNOME 47. This project ensures that your Adwaita icons reflect the same accent color as your GNOME theme, instead of the default blue, for a more cohesive and customized look.

GNOME 47 introduced a "color accent" feature to allow users to select a system-wide accent color. However, the default Adwaita icon theme does not automatically adapt to this accent color, leaving the icons in the default blue. Adwaita Colors fixes this by applying your chosen accent color to the icons.

In addition, I added MoreWaita icon folders and made them themed to allow for more extensive customization.

## Installation:

Clone the repository to your local machine:

```sh
git clone https://github.com/dpejoh/Adwaita-colors
```

To install the icons for your user, copy the Adwaita-colors folder to:

```sh
cp -r ./Adwaita-colors/* ~/.local/share/icons/
```

To install the icons globally for all users, use:

```sh
cp -r ./Adwaita-colors/* /usr/share/icons/
```
For immutable distros like Fedora Silverblue, the global installation is different, use:

```sh
cp -r ./Adwaita-colors/* /var/usrlocal/share/icons/
```

#### Arch Linux (AUR) packages

Release-based [adwaita-colors-icon-theme](https://aur.archlinux.org/packages/adwaita-colors-icon-theme):  
```sh
paru adwaita-colors-icon-theme
```
<sup>*Replace `paru` with `yay -S` or your favourite AUR helper install command.</sup>

Git-based [adwaita-colors-icon-theme-git](https://aur.archlinux.org/packages/adwaita-colors-icon-theme-git) for keeping up with all git changes between releases:  
```sh
paru adwaita-colors-icon-theme-git
```
<sup>*Replace `paru` with `yay -S` or your favourite AUR helper install command.</sup>

> [!TIP]
> Once the icons are installed, apply the theme through GNOME Tweaks.

## MoreWaita:

To install MoreWaita with Adwaita-colors:

- Run MoreWaita.sh after cloning the repository, or run command below directly.
- Use sudo for system-wide installation or on immutable distributions.

#### Without sudo:

```sh
wget -O MoreWaita.sh https://raw.githubusercontent.com/dpejoh/Adwaita-colors/main/MoreWaita.sh && chmod +x MoreWaita.sh && ./MoreWaita.sh
```
#### With sudo:
```sh
wget -O MoreWaita.sh https://raw.githubusercontent.com/dpejoh/Adwaita-colors/main/MoreWaita.sh && chmod +x MoreWaita.sh && sudo ./MoreWaita.sh
```

> [!NOTE]
> Arch Linux AUR packages integrate with MoreWaita automatically.

## Auto Match Adwaita-color with Accent Colors:

To automatically match your color accent with the Adwaita theme, you can install the "Auto Adwaita Colors" extension by [@celiopy](https://github.com/celiopy/auto-adwaita-colors).

### Installation:

You can install the extension directly from GNOME Shell Extensions:

[<img src="https://micheleg.github.io/dash-to-dock/media/get-it-on-ego.png" height="100">](https://extensions.gnome.org/extension/7529/auto-adwaita-colors/)

Or download the latest release from GitHub by running the following command:

```sh
wget https://github.com/celiopy/auto-adwaita-colors/releases/download/3.0/auto-adwaita-colors@celiopy.zip
```

Install the extension using GNOME:

```sh
gnome-extensions install --force "auto-adwaita-colors@celiopy.zip"
```

After installation, open the GNOME Extensions Manager and enable the extension from there.
