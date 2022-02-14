---
title: How it all started
description: Why was PolyMC created?
date: 2022-02-14
tags:
  - fork
  - multimc
---

PolyMC is a fork of the open source Minecraft launcher [MultiMC](https://multimc.org/).
If you don't know what a *fork* is, you can [read about it here](https://en.wikipedia.org/wiki/Fork_(software_development)).
Many forks exist, because (part of) a community around a project is unsatisfied.
PolyMC is also one of these forks.

# Change of course with MultiMC
The catalyst for this dissatisfaction was the account migration of Minecraft: Java Edition to Microsoft Authentication (MSA).
By design MSA is more restrictive for third-party launchers, as it needs a private token to communicate with Microsoft servers, in contrast to the rather open nature of Mojang authentication.
In September 2021 @peterix and the other MultiMC contributors have [released MultiMC 0.6.13][mmc-upd-2021-09].
This version finally brought MSA support to MultiMC and thus allowed people to log into their migrated Minecraft accounts.
Sadly this version marks the point where frustration in the community started to grow.

## The introduction of `DevLauncher`
Alongside MSA support the codebase was de-branded and all API keys were removed with version 0.6.13.
MultiMC was now called `DevLauncher` by default and doesn't work with MSA by default.
This was almost just a footnote in the changelog:

> ### Technical changes
> - The codebase continues to move towards being de-branded and harder to build as ‘MultiMC’ for third parties.

This started to produce issues around packaging.
MultiMC only provides portable binaries for the major platforms.
Compiling from source became a problem as it would produce a launcher with a different name and no support for MSA by default.
Packaging the *official* binaries became another problem, as they were available at a non-unique URL.
So if there was an updated the old binaries were just replaced by the new one, and there was no way of keeping track which version is actually being packaged.
Instead of addressing these issues, @peterix started to move users to his own distribution method by utilizing an update mechanism inside the launcher.
A `multimc-bin` package was provided for the AUR, which basically only contained a script to download the latest version from `multimc.org` and store it in the user's home folder.
Many people did not notice the difference and just used the launcher as is.

Later that year [a subsequent update was released][mmc-upd-2021-12], which refined the MSA support, fixed a few issues and completed the majority of the de-branding.
A few days later @peterix [filed a deletion request][del-req-mmc-git] on the AUR against the package `multimc-git` (maintained by now PolyMC head maintainer) with the following reasoning:

> - Stealing the client ID from MultiMC (which is in breach of Microsoft Identity Platform terms of service).
> - Trademark infringement (No you do not own MultiMC, and you don't get to slap that on anything you want).
> - Total disrespect for the original project and all of its contributors.

It was quickly dismissed by Arch Linux trusted users.

## Removal of Arch Linux packaging

As a response to @peterix' deletion request, [@binex-dsk][gh-binex-dsk], now one of the founders of PolyMC, has [filed a deletion][del-req-mmc-bin] as well as [an orphan request][orph-req-mmc-bin] against `multimc-bin`.
Arch Linux trusted users accepted the deletion request with the following comment:

> This is not an acceptable PKGBUILD: Installing an installer does have precedence in the AUR (i.e. minecraft-launcher) but installing an installer that just runs shell to install the latest version of the installer is not acceptible. 
> Please see minecraft-technic-launcher for inspiration.
> 
> Please feel empowered to fix these issues and re-submit (the underlying Git repo is not deleted).
> Do not resubmit this package unchanged.

This sparked a lot of controversy.
MutliMC officially discontinued Arch Linux support ([r/linux_gaming thread][r-linux_gaming-mmc-drop-aur], [r/linux thread][r-linux-mmc-drop-aur], [GitHub issue][mmc-gh-drop-aur]).

@Forkk on GitHub said:
> The new `multimc-bin` package that the AUR has replaced our official package with is broken and unsupported here. `multimc-git` is unsupported as well. No AUR packages will be supported any longer. Use the "generic" tarballs from the website instead.

So this marked the end of free packaging of MultiMC.
You could still install community packages from the AUR, but those were officially unsupported and who knew if they will work in the future.

# PolyMC was born
PolyMC 

[gh-binex-dsk]: https://github.com/binex-dsk
[mmc-upd-2021-09]: https://multimc.org/posts/0-6-13-update.html
[mmc-upd-2021-12]: https://multimc.org/posts/0-6-14-update.html
[del-req-mmc-git]: https://lists.archlinux.org/pipermail/aur-requests/2021-December/063454.html
[del-req-mmc-bin]: https://lists.archlinux.org/pipermail/aur-requests/2021-December/063455.html
[orph-req-mmc-bin]: https://lists.archlinux.org/pipermail/aur-requests/2021-December/063460.html
[r-linux_gaming-mmc-drop-aur]: https://www.reddit.com/r/linux_gaming/comments/riitbs/multimc_is_dropping_all_support_for_aur_packages/
[r-linux-mmc-drop-aur]: https://www.reddit.com/r/linux/comments/rie2oe/multimc_is_dropping_all_support_for_aur_packages/
[mmc-gh-drop-aur]: https://github.com/MultiMC/Launcher/issues/4352
