---
layout: layouts/main.njk
title: Home
background: ./src/img/background/home.jpg
hero:
  title: 'PolyMC'
  description: 'An Open Source Minecraft launcher with the ability to manage multiple instances, accounts and
  mods. Focused on user freedom and free redistributability.'
  image: 
    dark: ./src/img/screenshots/LauncherDark.png
    light: ./src/img/screenshots/LauncherLight.png
  background: 
  download: true
---

<div class="content">
  <div class="row row-reverse">
    <div class="column">
      <div>
        <h1>Modpack management</h1>
        <div class="subtitle">
          Install and launch modpacks easily, while keeping them clean.
          No longer do you need to manually install them, and updating feature is coming soon. PolyMC can do that for you, without installing tons of separate launchers.
        </div>
      </div>
    </div>
    <div class="column">
      {% image "Modpack Installer", "./src/img/screenshots/ModpackInstallLight.png", "./src/img/screenshots/ModpackInstallDark.png" %}
    </div>
  </div>

  <div class="row">
    <div class="column">
      <div>
        <h1>Download & Update Mods</h1>
        <div class="subtitle">
          <p>Are you sick of finding and adding that one mod you need? PolyMC is able to download & update individual mods from outside of modpacks using Modrinth and CurseForge.
        </div>
      </div>
    </div>
    <div class="column">
      {% image "Mod Installer", "./src/img/screenshots/ModInstallLight.png", "./src/img/screenshots/ModInstallDark.png" %}
      {% image "Mod Installer", "./src/img/screenshots/ModUpdateLight.png", "./src/img/screenshots/ModUpdateDark.png" %}
    </div>
  </div>

  <div class="row row-reverse">
    <div class="column">
      <div>
        <h1>Minecraft instance management </h1>
        <div class="subtitle">
          <p>Did your settings ever reset after launching an older version? Did you ever accidentally break a world because you opened it in an old version?
          Are you tired of manually switching mods for different versions, installing modloaders?<p>
          <p>PolyMC can help. Each Minecraft instance has its own folder, with separate mods, resourcepacks and other things.</p>
        </div>
        <br>
      </div>
    </div>
    <div class="column">
      {% image "Instance Settings", "./src/img/screenshots/PropertiesLight.png", "./src/img/screenshots/PropertiesDark.png" %}
    </div>
  </div>

  <div class="row">
    <div class="column">
      <div>
        <h1>Lightweight & Customizable</h1>
        <div class="subtitle">
          You don't need an embedded web browser for a game launcher. PolyMC uses the Qt toolkit, which requires little system resources. PolyMC also supports customizing the instance window and theme.
        </div>
      </div>
    </div>
    <div class="column">
      {% image "Mod Installer", "./src/img/screenshots/CustomizeLight.png", "./src/img/screenshots/CustomizeDark.png" %}
    </div>
  </div>
</div>
<div class="infobox top">

# Get involved

---

## Reddit
  
[![r/PolyMCLauncher](https://img.shields.io/reddit/subreddit-subscribers/PolyMCLauncher?label=r%2FPolyMCLauncher)](https://www.reddit.com/r/PolyMCLauncher/)

## Discord

To talk directly to us and get involved with development:

[![PolyMC Discord](https://img.shields.io/discord/923671181020766230?label=PolyMC%20Discord)](https://discord.gg/xq7fxrgtMP)

# Source code

---

PolyMC is focused on user freedom and free redistributability. All code is available on [the GitHub](https://github.com/PolyMC/PolyMC/) under the GPL-3 license.

[Source for this website](https://github.com/PolyMC/polymc.github.io) is hosted under the AGPL-3 License.

The logo and related assets are under the CC BY-SA 4.0 license.
</div>
