---
title: PolyMC 8.0 has been released
description: Play on blocked servers, download texture and shader packs, and more!
date: 2026-10-02
release_version: 8.0
minimum_macos_version: 11.0.0
legacy_macos_minimum_version: 10.14.0
mac_signature: b2B74lhzpCZO8IXHYU4KIGYczBlEQLH8z3ZmhqoF1qr3H6qwCqzdvd74zOXzKzFv6OFnoRAgTeXnceRtOyaYAg==
legacy_mac_signature: SsrJTwttkAd8qTO4KCmueJH9sWjrZcanMBaHHPdgqtlEtlJ2EpFSDTqfxVl4I6/pyibfUL6cKFsScAFBrVwYDQ==
tags:
  - release
---

This release contains some juicy new features, alongside UI enhancements, bug fixes for modpack providers and legacy versions, and most importantly: the ability to play on blacklisted servers, such as 6b6t!

## Features

- Servers that are otherwise blacklisted by Microsoft can now be played on, such as 6b6t. [@crueter](https://github.com/crueter) in [#1794](https://github.com/PolyMC/PolyMC/pull/1794)
- You can now download resource, texture, and shader packs from Modrinth or Curseforge. This works in beta versions too! [@crueter](https://github.com/crueter) in [#1804](https://github.com/PolyMC/PolyMC/pull/1804)
- The instance server list has been improved, now showing important data (player count, icons, etc.). [@Kaydax](https://github.com/Kaydax) in [#1730](https://github.com/PolyMC/PolyMC/pull/1730)
- Old versions of Minecraft with Forge installed previously did not work with modern Java 8 runtimes. The new "Ignore Forge security errors" option allows modern Java runtimes to bypass this and play old versions of Minecraft with Forge. [@crueter](https://github.com/crueter) in [#1795](https://github.com/PolyMC/PolyMC/pull/1795)
- You can now use the Loki Yggdrasil agent as a custom authentication alternative for versions 0.0.18a to 1.6.4. [@thedirtybubble](https://github.com/thedirtybubble) in [#1790](https://github.com/PolyMC/PolyMC/pull/1790)
- You can now use locally hosted HTTP metadata servers. [@JackOfNoneTrades](https://github.com/JackOfNoneTrades) in [#1762](https://github.com/PolyMC/PolyMC/pull/1762)
- Windows on ARM now has a setup executable (Windows 11 only). [@crueter](https://github.com/crueter) in [#1797](https://github.com/PolyMC/PolyMC/pull/1797)
- Linux AppImages can now automatically update themselves if a new upstream version is present. [@crueter](https://github.com/crueter) in [#1788](https://github.com/PolyMC/PolyMC/pull/1788)

## UI Improvements

- You can now add the same account name to multiple different services/hosts. [@prozacgod](https://github.com/prozacgod) in [#1727](https://github.com/PolyMC/PolyMC/pull/1727)
- Offline usernames are now checked for general validity, alongside previous length requirements. [@hustlerone](https://github.com/hustlerone) in [#1737](https://github.com/PolyMC/PolyMC/pull/1737)
- The offline login dialog now focuses on the username textbox by default. [@crueter](https://github.com/crueter) in [#1752](https://github.com/PolyMC/PolyMC/pull/1752)
- RAM allocation values below 1024 MiB now warn the user, but it can now be set as low as 8 MiB for very old versions. [@crueter](https://github.com/crueter) in [#1787](https://github.com/PolyMC/PolyMC/pull/1787)
- You can choose to ignore duplicated Java runtimes in the version selection screen. This is mostly useful on Linux. [@crueter](https://github.com/crueter) in [#1799](https://github.com/PolyMC/PolyMC/pull/1799)
- The log searching function will now automatically wrap its search if you reach the bottom or top. [@crueter](https://github.com/crueter) in [#1798](https://github.com/PolyMC/PolyMC/pull/1798)

## Bug Fixes

- The macOS icon has been updated to support macOS 26 and above. [@crueter](https://github.com/crueter) in [#1796](https://github.com/PolyMC/PolyMC/pull/1796)
- Font scaling on macOS has been fixed. [@crueter](https://github.com/crueter) in [#1796](https://github.com/PolyMC/PolyMC/pull/1796)
- Editing the maximum RAM allocation with a low minimum could cause strange behavior due to max >= min checks. [@crueter](https://github.com/crueter) in [#1791](https://github.com/PolyMC/PolyMC/pull/1791)
- Curseforge modpacks could potentially specify overrides that broke out of the dedicated staging path, which was a security risk. You are now warned if this is the case. [@crueter](https://github.com/crueter) in [#1805](https://github.com/PolyMC/PolyMC/pull/1805)
- Certain older texture packs may have had invalid or unreadable descriptions. Most of these will now display properly. [@crueter](https://github.com/crueter) in [#1808](https://github.com/PolyMC/PolyMC/pull/1808)
- ATLauncher modpacks now support NeoForge. [@Kaydax](https://github.com/Kaydax) in [#1759](https://github.com/PolyMC/PolyMC/pull/1759)
- Fixed ATLauncher modpacks crashing the launcher during installation if Liteloader was present. [@crueter](https://github.com/crueter) in [#1793](https://github.com/PolyMC/PolyMC/pull/1793)
- Fixed FTB modpacks being unable to download, or not being present in the modpack search menu. [@crueter](https://github.com/crueter) in [#1792](https://github.com/PolyMC/PolyMC/pull/1792)

**Full Changelog**: https://github.com/PolyMC/PolyMC/compare/7.1...8.0

You can [grab the latest download here](/download) for your respective platform.
