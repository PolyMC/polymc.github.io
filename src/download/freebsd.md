---
title: Download PolyMC for FreeBSD
eleventyNavigation:
  key: <i class="fa fa-freebsd" aria-hidden="true"></i>FreeBSD
  order: 3
---

<div class="infobox top">

# <img src="https://www.vectorlogo.zone/logos/freebsd/freebsd-icon.svg" height="20"/> FreeBSD

Source compilation:
  
```bash
git clone http://codeberg.org/glowiak/FreeBSD-Ports.git
cd FreeBSD-Ports/games/polymc
su root -c 'make install clean' # when it asks you to provide the patch destination, retype the second option
```
  
Binary installation (may be not up to date):
  
```bash
# add the repository, do everything as root
mkdir -p /usr/local/etc/pkg/repos
fetch -o /usr/local/etc/pkg/repos/delports.conf http://codeberg.org/glowiak/delports/raw/branch/master/delports.conf
pkg update
pkg install polymc
```

</div>
