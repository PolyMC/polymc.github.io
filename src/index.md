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
        <h1>Download Mods</h1>
        <div class="subtitle">
          <p>Are you sick of finding and adding that one mod you need? PolyMC is able to download individual mods from outside of modpacks using Modrinth and CurseForge.
        </div>
      </div>
    </div>
    <div class="column">
      {% image "Mod Installer", "./src/img/screenshots/ModInstallLight.png", "./src/img/screenshots/ModInstallDark.png" %}
    </div>
  </div>

  <div class="row row-reverse">
    <div class="column">
      <div>
        <h1>Minecraft instance management </h1>
        <div class="subtitle">
          <p>Did your settings ever reset after launching an older version? Did you ever accidentally break a world because you opened it in an old version?
          Are you tired of manually switching mods for different versions, installing modloaders?<p>
          <p>PolyMC can help. Each Minecraft instance has it's own folder, with separate mods, resourcepacks and other things.</p>
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
          You don't need an embedded web browser for a game launcher. PolyMC uses the Qt toolkit, which requires little system resources.
        </div>
      </div>
    </div>
    <div class="column">
      {% image "Mod Installer", "./src/img/screenshots/CustomizeLight.png", "./src/img/screenshots/CustomizeDark.png" %}
    </div>
  </div>

  <h1 style="text-align: center">Want to Get Involved?</h1>
<div class="row">
			<div class="column">
				<a class="brand-icon" href="https://www.reddit.com/r/PolyMCLauncher/">
					{% image "Reddit Logo", "./src/img/brands/Reddit_Mark.svg", "./src/img/brands/Reddit_Mark.svg" %}	
				</a>
				<div>
					<h2>Reddit</h2>
					<div class="subicon">
						Post and read posts all about PolyMc
					</div>
				</div>
			</div>
			<div class="column">
				<a class="brand-icon" href="https://discord.gg/xq7fxrgtMP">
					{% image "Discord Logo", "./src/img/brands/Discord-Logo-Color.svg", "./src/img/brands/Discord-Logo-Color.svg" %}
				</a>
				<div>
					<h2>Discord</h2>
					<div class="subicon">
						To talk directly to us and get involved with development.
					</div>
				</div>
			</div>
			<div class="column">
				<a class="brand-icon" href="/wiki/getting-involved/matrix/">
					{% image "Matrix Logo", "./src/img/brands/matrix-logo-light.svg", "./src/img/brands/matrix-logo-dark.svg" %}
				</a>
				<div>
					<h2>Matrix</h2>
					<div class="subicon">
						We have a Matrix Space which is bridged to the Discord server.
					</div>
				</div>
			</div>
			<div class="column">
				<a class="brand-icon" href="/wiki/development/">
					{% image "Github Logo", "./src/img/brands/Github_Mark_Light.svg", "./src/img/brands/Github_Mark_Dark.svg" %}
				</a>
				<div>
					<h2>Github</h2>
					<div class="subicon">
						PolyMC is focused on user freedom and free redistributability all code is available on Github.
					</div>
				</div>
			</div>
		</div>
</div>


