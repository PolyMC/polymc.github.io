---
title: PolyMC Update 1.4.3, now available
description: Notice
date: 2022-10-27
release_version: 1.4.3
minimum_macos_version: 10.14.0
mac_signature: --
tags:
  - release
---

## Notice
Due to most of our packaging getting pulled as a result of a misinformation campaign and fake malware scares, the methods for installing PolyMC have changed. Our packages on Scoop, Chocolatey, WinGet, PortableApps, Flathub, COPR, NixPkgs, Gentoo, and more have been either removed or otherwise affected, so PolyMC can no longer be reliably installed in these ways.

Currently, the recommended way of installing PolyMC on Windows is via the installer or the portable package provided in the GitHub releases section.

The recommended way of using PolyMC on Linux is now by using the AppImage, Flatpak, or compiling from source, since most distro repositories have removed PolyMC. If your distro still packages an up-to-date distribution of PolyMC then feel free to keep using it.

For Steam Deck, we recommend using the Flatpak. The installation method is described below, since PolyMC no longer appears in the Discover store for the time being.

If you need any help with installing PolyMC or with anything else PolyMC-related then as always you can get support on our Matrix room, our Discord server, or our Subreddit. These are linked in the project's [README](https://github.com/PolyMC/PolyMC/#help--support)

## Flatpak installation

1. Download [PolyMC-1.4.3.flatpak](https://github.com/PolyMC/PolyMC/releases/download/1.4.3/PolyMC-1.4.3.flatpak) from the GitHub releases
2. Open a terminal, navigate to your downloads folder (`cd ~/Downloads`)
3. Use one of these commands to install the Flatpak:
  - For a single-user install `flatpak install --user PolyMC-1.4.3.flatpak`
  - For a system-wide install `flatpak install --system PolyMC-1.4.3.flatpak`

## Changelog

### Added
- Curseforge workarounds by @LennyMcLennington in #1477 and #1482
  - Removed the non-working Curseforge key
  - Added a way to fetch a working Curseforge key at runtime

### Changed
- Added diagnostic logging for OAuth 2.0 token reply errors, and made it fail the activity by @Doggermelon in #1480

### Fixed
- Simplify abort handling and add missing emits by @flowln in d50f954
- Replaced the MSA Client ID, so Microsoft login works again by @LennyMcLennington in 95eac86
- Curseforge-related fixes by @LennyMcLennington in #1477 and #1482
  - Fixed an issue with the user agent being blocked by the Curseforge API
  - Fixed a crash caused by an unhandled JSON exception during instance importing
  - Fixed a bug that caused an event loop to never end when instance importing failed
  - Fixed a bug where the instance import dialog would not close after failure / being aborted


**Full Changelog**: https://github.com/PolyMC/PolyMC/compare/1.4.2...1.4.3

You can [grab the latest download here](/download) for your respective platform.