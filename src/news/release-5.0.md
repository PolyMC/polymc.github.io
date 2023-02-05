---
title: (SECURITY PATCH - PLEASE READ THIS NEWS POST FULLY TO STAY SAFE) PolyMC 5.0, now available
description: New features, bug fixes and an important patch for a security vulnerability.
date: 2023-02-04
release_version: 5.0
minimum_macos_version: 10.14.0
mac_signature: RmmJbGOAMTt2Q1ixvyYOLtYvBsCQhaY5+p8iNVM3l+AW4tlvHn4WV5uK1UIAhniTp5Um2yqXjFlJjk8IBhQHCw==
tags:
  - release
---

This release brings all of the features that were only available in develop until now, and more importantly a patch to address a security vulnerability.

## IMPORTANT notice regarding a security vulnerability in previous versions of the software

This version of PolyMC comes with a fix for a security vulnerability in the "import from zip" create instance option.

If for any reason you haven't updated to version **5.0 or above** do not use the "import from zip" option unless you are 100% sure that the file you're importing is safe (meaning you analysed it yourself and determined that it's safe, or you're the one who authored the file).

**Please** ensure in 'Help > About PolyMC' that you are running on at least version 5.0 before trying to use the "import from zip" option on any untrusted files.

As of this news post being created, Flathub still hasn't updated to 5.0, so seriously do make sure that you're on 5.0 before using the "import from zip" option. Flatpak users will likely have to wait up to a few hours for the PolyMC Flatpak to be updated on Flathub.

## What's Changed
* Fix variable substitution in pre launch/post exit hooks by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/952
* Hide the entire performance tab on the instance settings in non-Linux OSes by @flowln in https://github.com/PolyMC/PolyMC/pull/951
* Fix segmentation fault when using jar mods by @flowln in https://github.com/PolyMC/PolyMC/pull/956
* Fix filter in external resource pages not working by @flowln in https://github.com/PolyMC/PolyMC/pull/961
* Fix broken url in readme by @jopejoe1 in https://github.com/PolyMC/PolyMC/pull/958
* Fix adding multiple accounts in Qt6 by @flowln in https://github.com/PolyMC/PolyMC/pull/974
* Implement mod resolving for FTB by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/699
* Bump to C++17 by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/941
* Trash instances instead of deleting by @ryanccn in https://github.com/PolyMC/PolyMC/pull/549
* chore: update issue template to ask about Qt version by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1008
* fix: remove iconfix from libraries/README.MD by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1012
* Fix WinGet releaser by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/994
* Add root path detection on OpenBSD by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1019
* fix: work around ubuntu 22.04 openssl appimage issues by copying openssl libs by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1006
* chore: downgrade to Qt 6.3.0 on macos by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1014
* Remove orphaned metadata to avoid problems with auto-updating instances by @flowln in https://github.com/PolyMC/PolyMC/pull/1017
* Allow user to interrupt launch after 3 tries by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1018
* Fix some icon cache problems by @flowln in https://github.com/PolyMC/PolyMC/pull/920
* Run markdownlint on the markdown files by @txtsd in https://github.com/PolyMC/PolyMC/pull/909
* fix: Make world safety nag popup title text match the action by @budak7273 in https://github.com/PolyMC/PolyMC/pull/1039
* ATLauncher: Preliminary work towards pack updating by @jamierocks in https://github.com/PolyMC/PolyMC/pull/897
* Decode process lines as UTF-8 by @magneticflux- in https://github.com/PolyMC/PolyMC/pull/968
* Hide 'More news...' button if the news aren't loaded yet by @flowln in https://github.com/PolyMC/PolyMC/pull/1049
* check for java installs in PATH on windows by @TayouVR in https://github.com/PolyMC/PolyMC/pull/1068
* fix: update org.polymc.PolyMC.metainfo.xml.in to not make flatpak break next release by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1058
* Add "Open All" button to blocked mods dialog by @kumquat-ir in https://github.com/PolyMC/PolyMC/pull/919
* Disable "Check for Updates" while the game is running or if all mods are removed by @Gingeh in https://github.com/PolyMC/PolyMC/pull/1007
* Switch to new versioning scheme by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/992
* Only remove orphaned metadata once on mod page opening by @flowln in https://github.com/PolyMC/PolyMC/pull/1044
* Use QSharedPointer instead of own impl. for shared_qobject_ptr by @flowln in https://github.com/PolyMC/PolyMC/pull/1023
* Lazy-load type-specific instance settings by @flowln in https://github.com/PolyMC/PolyMC/pull/878
* Make Coremods / Mods seperation more clear by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1035
* fix(COPYING): fix COPYING.md by adding some missing copyright notices by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1073
* fix: fix urls on ftb legacy by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1087
* Refactor a bit EnsureMetadataTask and calculate hashes in a incremental manner by @flowln in https://github.com/PolyMC/PolyMC/pull/965
* Refactor resource models by @flowln in https://github.com/PolyMC/PolyMC/pull/1052
* Fix build by @flowln in https://github.com/PolyMC/PolyMC/pull/1094
* Never invalidate libraries cache entries by time elapsed by @flowln in https://github.com/PolyMC/PolyMC/pull/1080
* Move classpath definition into NewLaunch itself by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1067
* Ensure individual destination file path exists in FS::overrideFolder by @flowln in https://github.com/PolyMC/PolyMC/pull/1095
* Detect GameMode and MangoHud, disable if not present by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1034
* make the about dialog smaller by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1107
* Revert "Move classpath definition into NewLaunch itself" by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1111
* chore: update install-qt-action to v3 by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1114
* Fixed up a warning by @timoreo22 in https://github.com/PolyMC/PolyMC/pull/1113
* Reduce code duplication in tasks, fix some bugs and add some tests by @flowln in https://github.com/PolyMC/PolyMC/pull/966
* Some more UI / UX improvements to the mod downloader! by @flowln in https://github.com/PolyMC/PolyMC/pull/939
* Add basic resource pack parsing and fix issues by @flowln in https://github.com/PolyMC/PolyMC/pull/1105
* Use MC versions list instead of ad-hoc logic to filter by major version in the mod downloader by @flowln in https://github.com/PolyMC/PolyMC/pull/997
* Fix the mod updater not working as intended by @flowln in https://github.com/PolyMC/PolyMC/pull/1117
* fix meta by @dada513 in https://github.com/PolyMC/PolyMC/pull/1129
* fix(actions, win): only copy openssl libs on qt5 builds by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1130
* Emit correct signals on NetJob abort by @flowln in https://github.com/PolyMC/PolyMC/pull/1123
* Restructure tests by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1133
* Feature: Enable dark titlebar on Windows 10 (3) by @DavidoTek in https://github.com/PolyMC/PolyMC/pull/982
* fix: allow starting rd- versions by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1146
* Added a button to launch in Demo mode by @jopejoe1 in https://github.com/PolyMC/PolyMC/pull/903
* Use std::filesystem in some filesystem utils by @flowln in https://github.com/PolyMC/PolyMC/pull/1142
* Fix crash and memory leak because of Resources by @flowln in https://github.com/PolyMC/PolyMC/pull/1150
* Add basic texture pack parsing by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1108
* Allows double clicking to mark for download by @ErogigGit in https://github.com/PolyMC/PolyMC/pull/1165
* Improve language model by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1164
* Add early modpack updating system by @flowln in https://github.com/PolyMC/PolyMC/pull/894
* Replaced tomlc99 with tomlplusplus by @Trial97 in https://github.com/PolyMC/PolyMC/pull/1162
* Add missing includes to fix Qt 6.4 build by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1172
* Switch to QCommandLineParser by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1167
* Update winget.yml by @vedantmgoyal2009 in https://github.com/PolyMC/PolyMC/pull/1171
* Support more formatting codes by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1154
* Fix mod icon issues and change delegate for Modrinth Modpacks by @flowln in https://github.com/PolyMC/PolyMC/pull/1163
* Update capabilities before first-run wizard by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1183
* Improve default light and dark themes by @Protrikk in https://github.com/PolyMC/PolyMC/pull/1174
* fix: mod updating isn't upcoming anymore :p by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1185
* feat(actions): add codeql code scanning by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1177
* Multi-Arch Support by @Scrumplex in https://github.com/PolyMC/PolyMC/pull/1033
* Microsoft account only in https://github.com/PolyMC/PolyMC/pull/1175
* Merge Launch Buttons by @TayouVR in https://github.com/PolyMC/PolyMC/pull/1190
* Remove opted out versions from the download selector when using the 'Any' filter by @flowln in https://github.com/PolyMC/PolyMC/pull/1194
* make polymc build/work on platforms without std::filesystem, add macos-legacy package and remove old unnedeed hack by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1203
* fix: remove some unused libs by @DioEgizio in https://github.com/PolyMC/PolyMC/pull/1208
* change: Added diagnostic logging for OAuth 2.0 token reply errors, an… by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1480
* Curseforge workarounds and fixes by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1477
* Minor changes to curseforge workarounds by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1482
* Remove closed matrix rooms from README by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1490
* Have API key validators tolerate whitespace by @jdpatdiscord in https://github.com/PolyMC/PolyMC/pull/1494
* fix *bsd support by @unix-supremacist in https://github.com/PolyMC/PolyMC/pull/1500
* fix windows build by @binex-dsk in https://github.com/PolyMC/PolyMC/pull/1501
* Add Jinx by @HeyaGlitz in https://github.com/PolyMC/PolyMC/pull/1499
* fix: prevent stack overflow in ConcurrentTask by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1505
* Implement account per instance feature by @urFate in https://github.com/PolyMC/PolyMC/pull/1493
* Add Floppa :^) by @xslendix in https://github.com/PolyMC/PolyMC/pull/1510
* fix recursive crash on win64 by @jdpatdiscord in https://github.com/PolyMC/PolyMC/pull/1503
* Add a way to change the position of the cat. by @xslendix in https://github.com/PolyMC/PolyMC/pull/1508
* Add storage page to instances. by @xslendix in https://github.com/PolyMC/PolyMC/pull/1504
* Fix build fail on nix flake by @oluceps in https://github.com/PolyMC/PolyMC/pull/1531
* fix windows ci builds by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1538
* fix(ModrinthInstanceCreationTask): ignore files with invalid paths by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1537
* Fix Windows Qt6 builds by @LennyMcLennington in https://github.com/PolyMC/PolyMC/pull/1539

## New Contributors
* @budak7273 made their first contribution in https://github.com/PolyMC/PolyMC/pull/1039
* @magneticflux- made their first contribution in https://github.com/PolyMC/PolyMC/pull/968
* @TayouVR made their first contribution in https://github.com/PolyMC/PolyMC/pull/1068
* @kumquat-ir made their first contribution in https://github.com/PolyMC/PolyMC/pull/919
* @DavidoTek made their first contribution in https://github.com/PolyMC/PolyMC/pull/982
* @ErogigGit made their first contribution in https://github.com/PolyMC/PolyMC/pull/1165
* @Trial97 made their first contribution in https://github.com/PolyMC/PolyMC/pull/1162
* @vedantmgoyal2009 made their first contribution in https://github.com/PolyMC/PolyMC/pull/1171
* @Protrikk made their first contribution in https://github.com/PolyMC/PolyMC/pull/1174
* @jdpatdiscord made their first contribution in https://github.com/PolyMC/PolyMC/pull/1494
* @unix-supremacist made their first contribution in https://github.com/PolyMC/PolyMC/pull/1500
* @HeyaGlitz made their first contribution in https://github.com/PolyMC/PolyMC/pull/1499
* @urFate made their first contribution in https://github.com/PolyMC/PolyMC/pull/1493
* @xslendix made their first contribution in https://github.com/PolyMC/PolyMC/pull/1510
* @oluceps made their first contribution in https://github.com/PolyMC/PolyMC/pull/1531

**Full Changelog**: https://github.com/PolyMC/PolyMC/compare/1.4.3...5.0

You can [grab the latest download here](/download) for your respective platform.
