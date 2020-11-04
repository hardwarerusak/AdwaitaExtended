(Moved to GitLab: https://gitlab.com/hrdwrrsk/AdwaitaExtended) AdwaitaExtended
=====
**This master branch are for GNOME 3.38. this is also new home for the project because my old account has messed up**
> Using previous versions? there's a `gnome-3-34` and `gnome-3.36` branch

AdwaitaExtended is a stock Adwaita theme modified with:

- Uses compact variant by default `$sizevariant: compact;` (to make it better for low-resolution laptops)
- **New!** Adaptive font size in GNOME shell.
- Consistent GTK2 theme (finally!)
- Xfce4 support (with xfwm4 theme included)
- Budgie Desktop support ! (Requires Budgie Desktop 10.5.1 or latest git version)
> Unfortunately this theme doesn't shown in Budgie Desktop Settings. Use GNOME Tweaks to apply instead.
- MATE desktop support
> Although MATE is supported, currently there's no WM theme for Marco. I recommended to change default WM to metacity because it uses native GTK theming than legacy metacity-3 XML theming (although it's still available but disabled by default)
- Modifications/tweaks are done in `_tweaks.scss` instead modifying `_common.scss` directly, to keep in sync with upstream

### Screenies
![Light](/data/ss-light.png)
![Dark](/data/ss-dark.png)

### Installation
Clone this repo, and open directory with terminal and then:
```
meson build --prefix=/usr
sudo ninja -C build install
```
### Credits
- https://gitlab.gnome.org/GNOME/gtk (Adwaita GTK theme)
- https://gitlab.gnome.org/GNOME/gnome-themes-extra (Adwaita GTK 2 theme)
- https://gitlab.gnome.org/GNOME/gnome-shell (Adwaita shell theme)
- https://github.com/ubuntu/yaru (Upstream sync script)
- https://github.com/godlyranchdressing/gnome-theme-starter (Meson build template)
