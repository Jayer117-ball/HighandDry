<!-- Banner -->
<p align="center">
  <img src="https://raw.githubusercontent.com/Jayer117-ball/HighandDry/refs/heads/main/Banner%20Readme.png" alt="High and Dry Banner" />
</p>

<!-- Title -->
<h1 align="center">High & Dry</h1>
<p align="center"><b>Fallout: New Vegas — Wabbajack Modlist Installation Guide</b></p>

<!-- Link Bar -->
<p align="center">
  [
  <a href="https://www.nexusmods.com/newvegas/mods/88167" target="_blank" rel="noopener noreferrer">Nexus</a> |
  <a href="#-requirements">Requirements</a> |
  <a href="#️-step-by-step-installation">Installation</a> |
  <a href="#-post-installation-steps">Post-Installation</a> |
  <a href="#-updating-the-modlist">Updating</a> |
  <a href="https://github.com/Jayer117-ball/HighandDry/blob/main/Gameplay.md">Gameplay</a> |
  <a href="https://discord.gg/zV5zACunk3">Discord</a>
  ]
</p>

---

## Contents

- 📌 [Requirements](#-requirements)
  - [Choosing a Location](#choosing-a-location)
  - [Uninstalling the Games](#uninstalling-the-games)
  - [Installing the Games](#installing-the-games)
  - [Generating Fresh INI Files](#generating-fresh-ini-files)
- 🛠️ [Step-by-Step Installation](#️-step-by-step-installation)
- 🚀 [First-Time Launch](#-first-time-launch)
- 📦 [Post-Installation Steps](#-post-installation-steps)
  - 🔁 [Run 4GB Patch](#-run-4gb-patch)
  - 📜 [Install Vanilla UI Extension](#-install-vanilla-ui-extension)
  - 📜 [Install Cyberware 2281](#-install-cyberware-2281)
  - ⚙️ [DXVK](#️-dxvk)
- 📝 [Notes](#-notes)
- 🕹 [In-Game](#-in-game)
- ⚙️ [Optional Steps](#️-optional-steps)
  - 🧃 [BSA Decompressor](#-bsa-decompressor)
  - 🌃 [New Vegas Reloaded (NVR)](#-new-vegas-reloaded-nvr)
  - 🔧 [Shader Package](#-shader-package)
- 🎮 [Running the Game](#-running-the-game)
- 🔄 [Updating the Modlist](#-updating-the-modlist)
- 🎮 [Hotkeys](#-hotkeys---k-in-pause-menu-to-view-use-keybinder-mcm-to-configure-to-your-preferences-and-set-up)
- 🌵 [Modlist Overview](#-modlist-overview)
- 🆘 [Need Help?](#-need-help)

---

Welcome! This guide will help you install my **Fallout: New Vegas** modlist using **Wabbajack**. Whether you’re new to modding or just need some extra guidance, follow these steps carefully and in order, and you’ll be playing a fully modded New Vegas in no time!

---

## 📌 Requirements

Before we start, make sure you have:

- [Wabbajack](https://www.wabbajack.org/) (latest version)
- **At least 100 GB** of free space
- A **clean installation** of Fallout: New Vegas. Read each section below.

---

<details id="choosing-a-location">
<summary><strong>Choosing a Location</strong></summary>

<p>
A <strong>clean installation</strong> is not only required to get rid of any potential leftover mod files, but also to make sure the game is installed in a safe location. Here is what you need to know when choosing where to install your game:
</p>

<ul>
  <li><strong>Avoid any default Windows folders</strong>
    <ul>
      <li><code>C:\Program Files</code></li>
      <li><code>C:\Program Files (x86)</code></li>
      <li><code>Desktop</code></li>
      <li><code>Documents</code></li>
    </ul>
    <p>
      Users typically lack full write access to <code>Program Files</code>, while <code>Desktop</code> and <code>Documents</code> are often managed by <strong>OneDrive</strong>. This can cause many issues with the game and modding tools.
    </p>
    <p><strong>Example of a safe install location:</strong></p>
    <pre><code>C:\Games</code></pre>
  </li>

  <li><strong>Install on an SSD if possible</strong><br>
    Installing the game on an SSD will drastically improve loading times and reduce stuttering.
  </li>
</ul>

</details>

<hr>

<details id="uninstalling-the-games">
<summary><strong>Uninstalling the Games</strong></summary>

<p><em>If you never installed New Vegas before, go directly to the next section.</em></p>

<p>
As the games are available on Steam, GOG, and Epic Games, there are separate instructions for each version. You only need to follow the directions for the version(s) you have.
</p>

<h3>Steam</h3>

<blockquote>
  <p><strong>Note:</strong> If you already uninstalled the games, make sure to follow step 4 and 5 to ensure there are no leftovers.</p>
</blockquote>

<ol>
  <li>Open Steam and go to your <strong>Library</strong>.</li>
  <li>Find <strong>Fallout: New Vegas</strong> in the list.</li>
  <li>Right-click on it and select <strong>Manage</strong> → <strong>Uninstall</strong>.</li>
  <li>Navigate to <code>Steam\steamapps\common</code> and, if present, delete the <strong>Fallout New Vegas</strong> folder.</li>
  <li>Navigate to <code>Documents\My Games\FalloutNV</code> and delete all INI files inside it.</li>
</ol>

<h3>GOG</h3>

<ol>
  <li>Open GOG and go to your <strong>Library</strong>.</li>
  <li>Find <strong>Fallout: New Vegas</strong> in the list.</li>
  <li>Right-click on it and select <strong>Manage Installation</strong> → <strong>Uninstall</strong>.
    <ul>
      <li>If you used an offline installer then run the <code>unins000.exe</code> file in the game's <strong>Root</strong> folder.</li>
    </ul>
  </li>
  <li>Navigate to <code>Documents\My Games\FalloutNV</code> and delete all INI files inside it.</li>
</ol>

<h3>Epic Games</h3>

<blockquote>
  <p><strong>Note:</strong> If you already uninstalled the games, make sure to follow step 4 to ensure there are no leftovers.</p>
</blockquote>

<ol>
  <li>Open the Epic Games Launcher and go to your <strong>Library</strong>.</li>
  <li>Find <strong>Fallout: New Vegas</strong> in the list.</li>
  <li>Click on the 3 dots and select <strong>Uninstall</strong> from the menu.</li>
  <li>Navigate to <code>Documents\My Games\FalloutNV_Epic</code> and delete all INI files inside it.</li>
</ol>

</details>

<hr>

<details id="installing-the-games">
<summary><strong>Installing the Games</strong></summary>

<p>
As the games are available on Steam, GOG, and Epic Games, there are separate instructions for each version. You only need to follow the directions for the version(s) you have.
</p>

<h3>Steam</h3>

<h4>Creating a New Steam Library</h4>

<blockquote>
  <p>
    <strong>Important:</strong> It is strongly recommended to install the games outside of any default Windows folders (such as <code>Program Files (x86)</code>), as the strict Windows file protections of these folders can break certain mods/tools.
    <br><br>
    Instead, we will use the <strong>Steam Library Setup Tool</strong> to create a new Steam library folder outside of any default Windows folders.
  </p>
</blockquote>

<p>
If you already have Steam installed outside of any default Windows folders, go directly to step 1 of the next section and install the games to your custom Steam library.
</p>

<ol>
  <li>Completely exit Steam using Task Manager or the system tray.</li>
  <li>Download the <code>steam_library_setup_tool-3.2.exe</code> file.</li>
  <li>Run the tool and add a new entry by clicking <strong>Add Row</strong>.</li>
  <li>Type the desired path under <strong>Path</strong> (e.g. <code>C:\Games\Steam</code>).</li>
  <li>Click <strong>Accept</strong>, then <strong>Yes</strong> if prompted to create a new folder.</li>
  <li>The tool will ask to exit — select <strong>OK</strong>.</li>
</ol>

<ol>
  <li>Open Steam and go to your <strong>Library</strong>.</li>
  <li>Find <strong>Fallout: New Vegas</strong> in the list and select <strong>Install</strong>.</li>
  <li>Under <strong>Install to</strong>, select the library folder created with the tool.</li>
  <li>Select <strong>Next</strong> and wait for the installation to finish.</li>
</ol>

<blockquote>
  <p><strong>Note:</strong> If you do not see your new library, restart your PC.</p>
</blockquote>

<h3>GOG</h3>

<ol>
  <li>Open GOG and go to your <strong>Library</strong>.</li>
  <li>Find <strong>Fallout: New Vegas</strong> in the list and select <strong>Install</strong>.</li>
  <li>Set the install location to a folder of your choice.</li>
  <li>
    <strong>Required:</strong> Install the game outside of any default Windows folders
    (e.g. <code>Program Files (x86)</code>).
  </li>
</ol>

<h3>Epic Games</h3>

<ol>
  <li>Open the Epic Games Launcher and go to your <strong>Library</strong>.</li>
  <li>Find <strong>Fallout: New Vegas</strong> in the list.</li>
  <li>Click on the game to install it.</li>
  <li>
    <strong>Required:</strong> Install the game outside of any default Windows folders
    (e.g. <code>Program Files (x86)</code>).
  </li>
</ol>

</details>

<hr>

<details id="generating-fresh-ini-files">
<summary><strong>Generating Fresh INI Files</strong></summary>

<ol>
  <li>
    Run the game from <strong>Steam</strong> / <strong>GOG Galaxy</strong>, or run
    <code>FalloutNVLauncher.exe</code> directly from the game files if you are using an offline copy.
  </li>

  <li>
    Click <strong>OK</strong> on both pop-ups that say
    <strong>Detecting Video Hardware</strong>.
  </li>

  <li>
    If there are no pop-ups:
    <ul>
      <li>
        Navigate to <code>Documents\My Games\FalloutNV</code>
      </li>
      <li>
        Delete all INI files inside the folder
      </li>
      <li>
        Relaunch the game and try again
      </li>
    </ul>
  </li>

  <li>
    Click <strong>OK</strong>, then select <strong>Exit</strong>.
  </li>
</ol>

</details>

<hr>

- The latest **VC++ Redistributables**:  
  👉 [VC++ AIO Download](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/)  
  → Extract the archive and run `install_all.bat` as administrator
- DirectX End-User Runtime:  
  👉 [DirectX Download](https://www.microsoft.com/en-us/download/details.aspx?id=35)
- Read the **Introduction** and **Setup** pages from the [Viva New Vegas Guide](https://vivanewvegas.moddinglinked.com/intro.html).
- Restart your PC

---

## 🛠️ Step-by-Step Installation

### 1. Download Wabbajack
Go to the [Wabbajack website](https://www.wabbajack.org/) and download the latest version.

### 2. Create a Modding Folder
Create a new folder **outside** of default Windows folders (e.g., **not in Documents or Program Files**).

Example: C:\Modding\Wabbajack

### 3. Run Wabbajack
Move `Wabbajack.exe` to your new folder and run it.

### 4. Select Installation Location
Create a **separate**, empty folder for the modlist installation.

Example: C:\Modding\HighAndDry


### 5. Begin Installation
In Wabbajack:
- Select your installation and download folders
- Click **Begin Installation**
- If you don’t have a Nexus Premium account, you’ll need to manually download each mod

### 6. Finish Installation
- ✅ If successful: You'll see **"Installation Complete"**
- ❌ If failed: Log in to Nexus Mods again via Wabbajack and try reinstalling
- ❌ If failed: Validate files in Steam

---

## 🚀 First-Time Launch

- Launch **Fallout: New Vegas** through **Steam** once to generate config files
- Let it detect your resolution, then close it
- Now you must **always** launch the game via **Mod Organizer 2**

---

## 📦 Post-Installation Steps

### 🔁 Run 4GB Patch

1. Open **Mod Organizer 2** that shipped with High and Dry  
2. Click the Executable drop down and click on **FNVPatch**
- Check to see if the Binary path is correct before running the patcher. Yours should point to wherever you installed the list. And the **"Start in"** path points to your **game folder**. Example for mine below.
- ![Example](https://raw.githubusercontent.com/Jayer117-ball/HighandDry/refs/heads/main/4GB%20Patch%20Fixed.png)
3. MO2 will load the application
4. After running `FNVpatch` — it should confirm:  
   `FalloutNV.exe patched!`

### 📜 Install Cyberware 2281

1. Download [Cyberware 2281](https://mod.pub/falloutnv/15-cyberware-22810)
2. Install it manually through **Mod Organizer 2**
3. Place it anywhere in the **Overhauls** separator
4. Hide or delete Cyberware OWB. I merged it with the main Cyberware.esm in my patch mod.

### ⚙️ DXVK

- In **Mod Organizer 2** open the **Essentials** separator and read through the notes regarding each version of DXVK and decide the version that suits your PC.
- **Default (Recommended):** DXVK 2.6.1
- Others: DXVK 2.6.2 HDR, 1.10.1 (Intel GPU), and 1.10.3 (GPU w/out Vulkan support)
- You don't need DXVK, but if your setup can run it, I recommend you use it. NVR plays well with it too.

---

## 📝 Notes

- Expand the **separators in MO2** and read notes on individual mods. Most notes can be expanded for more information.
- Some mods have extra features or useful usage tips
- Click here to read about mods that High & Dry includes -> [High & Dry Gameplay](https://github.com/Jayer117-ball/HighandDry/blob/main/Gameplay.md)
- Crash logs are located here: MO2 > Overwrite > Root

---

## 🕹 In-Game

1. Complete the intro with Doc. DO NOT LEAVE THE HOUSE.
2. Save and exit the game. Reload your save.
3. **Pip boy real time map** and **Condition Meter Icons** should be working correctly.
4. Set up hotkeys for grenades, mines, and/or throwables
5. Equip the weapon > hold "Z" or grab and press G, H, or B and it should create a hotkey for that weapon. Press again to switch back to your previous weapon.

---

## ⚙️ Optional Steps

### 🧃 BSA Decompressor

- FYI: Whenever you do a clean install of New Vegas, you will have to do this step again
- Go to your installation folder
- Run `FNV BSA Decompressor.exe`  
→ Reduces load times and stutters

### 🌃 New Vegas Reloaded (NVR)

1. Download the **latest Nightly Build** from [TES Reloaded Discord](https://discord.com/invite/BYY7SNfQeJ)
2. In MO2:
- Switch to one of the NVR profiles
- Manually install NVR and drag it to the **"Place NVR Here"** separator
3. Enable either **Hikikomori NVR** or **Caffiene NVR**, your preference.
  - There are a few performance mods for both presets

### 🔧 Shader Package

This mod is optional but it does fix directional reflections in your game, I recommend it.

1. Navigate to:  
Documents\My Games\FalloutNV
2. Open `RendererInfo.txt`
3. Find your **shader model** (2nd line from bottom)
4. Go into **MO2** and locate your shader package number in the **shader package separator** under **Optionals**
5. Enable the box and that's it.

---

## 🎮 Running the Game

There are **4 profiles**: (soon to be 5)

- **Normal:** 2K textures
- **Hardcore:** Same as Normal + extra hardcore mods
- **Normal NVR** 2k textures with NVR mods enabled (still need to enable a preset)
- **Hardcore NVR** Same as Normal + extra hardcore + NVR mods (still need to enable a preset)
- **Performance:** WIP

🔹 To play, make sure **High & Dry** is selected in the MO2 drop down  
❌ Do **NOT** use Fallout Launcher or NVSE directly

- Fallout Launcher will appear the **first time** — that's okay
- Missing profile-specific game INI files — that's okay  
  - Click OK and continue
- Close it and relaunch the game via MO2

---

## 🔄 Updating the Modlist

To update:

1. For any manually added mods:
- Add `[NoDelete]` to the front of a mod name.
  - Add `[NoDelete]` to:
    - Vanilla UI Extension
    - New Vegas Reloaded
    - Cyberware
2. Re-download the Wabbajack file — it will update automatically
4. Re-run the 4GB Patch. (it may need to be re-run)
5. Complete #2 & #3 from the previous "In-Game" section.

---

## 🎮 Hotkeys - K in pause menu to view. Use Keybinder MCM to configure to your preferences and set up.

| Action | Key / Button | Action | Key / Button | Action | Key / Button |
|:---:|:---:|:---:|:---:|:---:|:---:|
| Pause Menu | `ESC` | Menu Overhauls | `N` | Mod Configuration Menu (MCM) | `M` |
| Achievements Menu | `T` | HUD Editor | ▲ *(Up Arrow, bottom right)* | Move | `WASD` |
| Activate / Interact | `E` | Open Pip-Boy | `Tab` | Ready / Reload weapon | `R` |
| Sneak *(Hold to Prone)* | `L-Ctrl` | Sprint | `L-Shift` | Hold Breath | `L-Alt` |
| Toggle Always Run | `Caps Lock` | Toggle Always Move | `Q` | Jump | `Space` |
| Change View (1st/3rd Person) | `F` | Wait | `T` | iHud toggle | `I` |
| V.A.T.S. | `V` | Toggle Quest Log | `J` | Weapon Hotkey | `G` |
| Weapon Hotkey | `H` | Weapon Hotkey | `B` | Ammo Check | `O` |
| Weapon Condition Check | `P` | Lean Left While Aiming | `X + Q` | Lean Right While Aiming | `X + E` |
| JIP Follower Commands (toggle) | `Hold 1` | Follower Wait *(Hold to make them follow)* | `2` | Real Time Pip Boy Map (Toggle) | `3` |
| Bullet Time | `Mouse Button 4` | Weapon Wheel | `Mouse Button 3` |  |  |


---

## 🌵 Modlist Overview

Here I will go over important parts of the modlist to help you better understand this list!  
Using **Wabbajack**, the list provides a streamlined installation process along with modern visual upgrades, gameplay refinements, and quality-of-life improvements — all while preserving the spirit and tone of New Vegas.

### ✨ Features
**Plug-and-play installation** through Wabbajack 
- **Updated visuals:** I include top of the line visual overhauls that make the mojave beautiful, but dangerous. There are so many visual upgrades but here I want to highlight some notable ones.
- **Early Loaders:** are the visual baseline mods that I have built the list off of.
- **Visuals:** you'll see a majority of the visual upgrades that are packed into BSA's. This list also offers NVR as an optional visual upgrade with shadows, tonemapping, increase LOD range, parrallax, and more. 
- **User Interface:** I've spent the majority of my time modifing the UI. It's clean, consistent, colorful where it needs to be, more detailed with widgets, icons, enemy health and boss bars. I hope you enjoy the UI as much as I do.
- **Gameplay enhancements:** Gameplay for this list has changed a lot, but the core is that same. Fun and challenging. This isn't a hardcore list, but it's a list that will challenge you and keep you on your toes. - Enemies are de-leveled - Ghouls are tougher and cause radiation damage - NPC's will feel real, they'll be able to pick up weapons much quicker, react to situations faster, use cover MUCH more, prone, use chems, sprint, react to gunshots, and work as a team to take you down
  - Damage is redone with damage and health scaling, reworking the DT and DR mechanics to make armor truly matter
  - No more bullet sponges or meaningless protection 
  - Loot is more scarce with Famine
  - Just Assorted Mods adds a weapon wheel for quick weapon selection, bullet time, dynamic crosshair, visual objectives
  - More implants with Cyberware 2281
- **Content:** I've also added some new content here and there but not a lot. - A World of Pain Revised adds more locations to explore and quests in an immersive way - Dry Wells - A legion expansion - Long 15 - NCR expansion - Living Desert makes the Mojave feel more alive with more NPC's and scripted events along your travels - Many location overhauls that I personally like and patched to work together - Lucky 38 Suite Overhaul (my own creation)
- **Animations:** Movement feels smoother and your character feels more alive

### 🧭 Philosophy
The goal of **High and Dry** is to provide a **stable, lore-friendly, and atmospheric** experience that feels like a remastered New Vegas without compromising what makes the game iconic. Every mod is chosen and tested with an emphasis on **compatibility, performance, and consistency** to ensure a smooth, less-crash playthrough. This is all starts with Viva New Vegas. A modlist that is now an essential and highly regarded in the FNV community *Shoutout to ModdlingLinked*.

---

## 🆘 Need Help?

- **Game won’t launch?**  
Make sure you have the **latest VC++ Redistributables**

- **Still still won’t launch?**  
Make sure the **4GB patch** was applied!

- **Still still still won’t launch?**  
Don’t install FNV to `Program Files` — [learn how to change it](https://vivanewvegas.moddinglinked.com/setup.html)

- **Still still still STILL won’t launch?**  
Make sure your Fallout New Vegas game folder is completely clean with nothing extra inside.

- **Still still still still STILL won’t launch?**  
Hey, it happens! Join the [Discord](https://discord.gg/zV5zACunk3), read the FAQ, and ask in the correct channel

---
