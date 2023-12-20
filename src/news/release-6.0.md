---
title: PolyMC 6.0, now available
description: Added support for Authlib-Injector, plus various bug fixes.
date: 2023-12-20
release_version: 6.0
minimum_macos_version: 10.14.0
mac_signature: ybdNZFYi4qSkJoFzDpvrlYQt1LeZ/OG1ANeX0/v4r2UnIvideVheSSsl++Je2bgQm88PqOqtggrnQepDj4I8Cw==
tags:
  - release
---

## What's Changed

### Added
* Add support for authlibinjector by @Kaydax in https://github.com/PolyMC/PolyMC/pull/1598

### Changed
* Add CMake option to enable stricter DRM by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1595
* don't set arbitrary minimum for jvm memory by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1615

### Fixed
* fix: change windows legacy builds to 64 bit by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1555
* Fix compile error on FreeBSD by @glowiak in https://github.com/PolyMC/PolyMC/pull/1560
* Clean up codebase and fix bug by @jdpatdiscord in https://github.com/PolyMC/PolyMC/pull/1575
* Fix bug, fix more warnings (See commit description) by @jdpatdiscord in https://github.com/PolyMC/PolyMC/pull/1576
* Update to Java 8 by @HeyaGlitz in https://github.com/PolyMC/PolyMC/pull/1581
* Fix build on Qt 6.6.0 by @binex-dsk in https://github.com/PolyMC/PolyMC/pull/1612
* Allow compilation on 32-bit by @jdpatdiscord in https://github.com/PolyMC/PolyMC/pull/1608
* fix hang when importing certain modpacks by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1616
* Fix MSA profile fetching by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1621
* Create offline mode accounts with consistent Uuids by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1622

## New Contributors
* @Spongecade made their first contribution in https://github.com/PolyMC/PolyMC/pull/1605
* @Kaydax made their first contribution in https://github.com/PolyMC/PolyMC/pull/1598

**Full Changelog**: https://github.com/PolyMC/PolyMC/compare/5.1...6.0

You can [grab the latest download here](/download) for your respective platform.
