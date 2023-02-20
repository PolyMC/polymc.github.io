---
title: (ANOTHER SECURITY VULNERABILITY - READ TO STAY SAFE) PolyMC 5.1, now available
description: Bug fixes and patch for a security vulnerability.
date: 2023-02-19
release_version: 5.1
minimum_macos_version: 10.14.0
mac_signature: r0T8ecyH7XTXD+3ZbgcUVRP6vxvoAWD8EqtHz67WqEY1yuDuGQH+q2XsmaSpV/dGsvVKnYJLIsk+VUgXe+iOCA==
tags:
  - release
---

This new version of PolyMC patches a security vulnerability in the software's zip file handling. Don't use the 'import from zip' option on versions of the software older than 5.1.

Other changes are a fix to importing FTB packs, a fix for the modrinth pack list being formatted wrong, and a fix for copying instances on Unix-like systems.

## What's Changed
* fix(MMCZip): ignore invalid file paths in extractSubDir by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1546
* fix: handle single files in copy tasks by @Doggermelon in https://github.com/PolyMC/PolyMC/pull/1526
* fix: Make modrinth text layout not be weird by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1548
* Clean & Compress Floppas by @KaspianDev in https://github.com/PolyMC/PolyMC/pull/1541
* Fix instance copy on Linux and macOS by flowln in https://github.com/PolyMC/PolyMC/pull/1552

## New Contributors
* @Doggermelon made their first contribution in https://github.com/PolyMC/PolyMC/pull/1526
* @KaspianDev made their first contribution in https://github.com/PolyMC/PolyMC/pull/1541

**Full Changelog**: https://github.com/PolyMC/PolyMC/compare/5.0...5.1

You can [grab the latest download here](/download) for your respective platform.
