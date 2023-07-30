---
title: Download PolyMC for Linux
eleventyNavigation:
  key: <i class="fa fa-linux" aria-hidden="true"></i>Linux
  order: 3
---

<div class="download-content">
  <div class="row">
    <div class="column">
      <div>
        <h1>Linux Download</h1>
        <br>
        <a class="button is-big" href="https://flathub.org/apps/details/org.polymc.PolyMC">Install from FlatHub</a>
        <a class="button is-big" href="https://github.com/PolyMC/PolyMC/releases/download/{{version.current}}/PolyMC-Linux-{{version.current}}-x86_64.AppImage">Download (AppImage)</a>
        <a class="button is-big" href="https://github.com/PolyMC/PolyMC/releases/download/{{version.current}}/PolyMC-Linux-{{version.current}}.tar.gz">Download (tar.gz)</a>
        <a class="button is-big" href="https://github.com/PolyMC/PolyMC/releases/download/{{version.current}}/PolyMC-Linux-portable-{{version.current}}.tar.gz">Download Portable (tar.gz)</a>
        <a class="button is-big" href="https://github.com/PolyMC/PolyMC/releases/download/{{version.current}}/PolyMC-Linux-Qt6-{{version.current}}.tar.gz">Download (Qt 6, tar.gz)</a>
        <a class="button is-big" href="https://github.com/PolyMC/PolyMC/releases/download/{{version.current}}/PolyMC-Linux-Qt6-portable-{{version.current}}.tar.gz">Download Portable (Qt 6, tar.gz)</a> 
     </div>
    </div>
    <div class="column">
      {% image "Modpack Installer", "./src/img/screenshots/LauncherLight.png", "./src/img/screenshots/LauncherDark.png" %}
    </div>
  </div>
</div>

<div class="infobox top">

# <img src="https://www.vectorlogo.zone/logos/archlinux/archlinux-icon.svg" height="20"/> Arch Linux / Manjaro

There are several AUR packages available:  
[![polymc](https://img.shields.io/badge/aur-polymc-blue)](https://aur.archlinux.org/packages/polymc/)  
[![polymc-bin](https://img.shields.io/badge/aur-polymc--bin-blue)](https://aur.archlinux.org/packages/polymc-bin/)  
[![polymc-git](https://img.shields.io/badge/aur-polymc--git-blue)](https://aur.archlinux.org/packages/polymc-git/)

```bash
# stable source package:
yay -S polymc
# stable binary package:
yay -S polymc-bin
# latest git package:
yay -S polymc-git
```

If you want to use Qt 5 to build the packages instead:

```bash
# stable Qt 5 source package:
yay -S polymc-qt5
# stable Qt 5 binary package:
yay -S polymc-qt5-bin
# latest Qt 5 git package:
yay -S polymc-qt5-git
```

You can replace yay -S with your preferred [AUR helper's](https://wiki.archlinux.org/title/AUR_helpers) install command.

</div>

<div class="infobox top">

# <img src="https://www.vectorlogo.zone/logos/nixos/nixos-icon.svg" height="20" /> Nix

A [Nix derivation](https://github.com/PolyMC/PolyMC/blob/develop/nix/NIX.md) is available.

</div>

<div class="infobox top">

# <img src="https://www.vectorlogo.zone/logos/getfedora/getfedora-icon.svg" height="20"/> RPM

An RPM package is available [on COPR](https://copr.fedorainfracloud.org/coprs/polymc/polymc/):
  
```bash
dnf copr enable polymc/polymc
```

</div>

<div class="infobox top">

# <img src="https://www.gentoo.org/assets/img/logo/gentoo-signet.svg" height="20"/> Gentoo Linux

ebuilds for PolyMC can be downloaded from the [polymc](https://git.swurl.xyz/PolyMC/overlay) overlay.

Write the following to `/etc/portage/repos.conf/polymc.conf`:

```ini
[polymc]
location = /var/db/repos/polymc
sync-type = git
sync-uri = https://git.swurl.xyz/PolyMC/overlay.git
```

If you want to build and install the latest version from git, then unmask the 9999 ebuild:

```bash
echo "=games-action/polymc-9999 **" | sudo tee -a /etc/portage/package.accept_keywords/polymc
```

If your `package.accept_keywords` is simply a file, remove the `/polymc` at the end.

Finally, sync the overlay:

```bash
sudo emaint sync -r polymc
```

And emerge:

```bash
sudo emerge -a polymc
```

</div>

<div class="infobox top">

# <img src="https://voidlinux.org/assets/img/void_bg.png" height="20"/> Void Linux

First you need to get the repo:
```bash
echo 'repository=https://xslendi.xyz/void' | sudo tee /etc/xbps.d/69-polymc.conf
```
Then you need to sync and install:
```bash
sudo xbps-install -S PolyMC-qt5
```
Or, if you have `xtools` installed:
```bash
xi PolyMC-qt5
```

</div>
