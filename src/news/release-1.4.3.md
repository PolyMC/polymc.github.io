---
title: Major Bugfix 1.4.3, now available
description: Squashed bugs
date: 2022-10-27
release_version: 1.4.3
minimum_macos_version: 10.14.0
mac_signature: T9oVKld9HpjSCd3BbecRHUhyY8Yx4cLpWclvlE8+PYvNg7BQc6wnjFmxNYYWjAWUOv50WstOVG14Sm4hGLJzBg==
tags:
  - release
---

It has been a good minute.
This release is a bugfix to address issues that have surfaced within the past week. 
Mostly pertaining to the online services used within the PolyMC client.
More features are on the way, just not in this release.

## Changelog

### Added
- Curseforge workarounds by @LennyMcLennington in #1477 and #1482
  - Removed the non-working Curseforge key
  - Added a way to fetch a working Curseforge key at runtime

### Changed
- Added diagnostic logging for OAuth 2.0 token reply errors, and made it fail the activity by @Doggermelon in #1480

### Fixed
- Simplify abort handling and add missing emits by @flowln in d50f954
- Curseforge-related fixes by @LennyMcLennington in #1477 and #1482
  - Fixed an issue with the user agent being blocked by the Curseforge API
  - Fixed a crash caused by an unhandled JSON exception during instance importing
  - Fixed a bug that caused an event loop to never end when instance importing failed
  - Fixed a bug where the instance import dialog would not close after failure / being aborted

## Installation
The methods of installation have been temporarily limited, please see our github (below) to download the latest version, you can read more [here](/news/what-happened/).

**Full Changelog**: https://github.com/PolyMC/PolyMC/compare/1.4.2...1.4.3

You can [grab the latest download here](/download) for your respective platform.
