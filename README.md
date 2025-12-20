
![Banner Readme](https://github.com/user-attachments/assets/cd44d8cf-4901-48e6-9577-daa3a7deb2fc)

# High and Dry Modlist Installation Guide

Welcome! This guide will help you install my **Fallout: New Vegas** modlist using **Wabbajack**. Whether you’re new to modding or just need some extra guidance, follow these steps carefully and in order, and you’ll be playing a fully modded New Vegas in no time!

---

## 📌 Requirements

Before we start, make sure you have:

- [Wabbajack](https://www.wabbajack.org/) (latest version)
- A **clean installation** of Fallout: New Vegas (no mods installed yet)
- **At least 100 GB** of free space
- The latest **VC++ Redistributables**:  
  👉 [VC++ AIO Download](https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/)  
  → Extract the archive and run `install_all.bat` as administrator
- DirectX End-User Runtime:  
  👉 [DirectX Download](https://www.microsoft.com/en-us/download/details.aspx?id=35)
- Read the **Introduction** and **Setup** pages from the [Viva New Vegas Guide](https://vivanewvegas.moddinglinked.com/intro.html). There is a lot of useful information there if you are new to MO2 or if you are an experienced user.
- Restart your PC

---

## 🛠️ Step-by-Step Installation

### 1. Download Wabbajack

Go to the [Wabbajack website](https://www.wabbajack.org/) and download the latest version.

### 2. Create a Modding Folder

Create a new folder **outside** of default Windows folders (e.g., **not in Documents or Program Files**).

Example:
C:\Modding\Wabbajack

### 3. Run Wabbajack

Move `Wabbajack.exe` to your new folder and run it.

### 4. Select Installation Location

Create a **separate**, empty folder for the modlist installation.

Example:
C:\Modding\HighAndDry

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

- Launch **Fallout: New Vegas through Steam** once to generate config files
- Let it detect your resolution, then close it
- Always launch the game via **Mod Organizer 2**

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

### 📜 Install Vanilla UI Extension

1. Download [Vanilla UI Extension](https://www.moddb.com/mods/vanilla-ui-extension/downloads/vanilla-ui-extension-10)
2. Install it manually through **Mod Organizer 2**
3. Place it **after Vanilla UI Plus** in the left pane

### 📜 Install Cyberware 2281

1. Download [Cyberware 2281](https://mod.pub/falloutnv/15-cyberware-22810)
2. Install it manually through **Mod Organizer 2**
3. Place it anywhere in the **Overhauls** separator
4. Hide or delete Cyberware OWB. I merged it with the main Cyberware.esm in my patch mod.

### ⚙️ DXVK or Heap Replacer (Choose One)

- In **Mod Organizer 2** open the **Essentials** separator and read through the notes regarding each version of DXVK and Heap Replacer and decide the version that suits your PC.
- **Default (Recommended):** DXVK 2.6.1
- Others: DXVK 2.6.2 HDR, 1.10.1 (Intel GPU), and 1.10.3 (GPU w/out Vulkan support)

---

## 📝 Notes

- Expand the **separators in MO2** and read notes on individual mods. Most notes can be expanded for more information.
- Some mods have extra features or useful usage tips

---

## ⚙️ Optional Steps

### 🧃 BSA Decompressor

- Go to your installation folder
- Run `FNV BSA Decompressor.exe`  
→ Reduces load times and stutters

### 🌃 New Vegas Reloaded (NVR)

1. Download the **latest Nightly Build** from [TES Reloaded Discord](https://discord.com/invite/BYY7SNfQeJ)
2. In MO2:
- Switch to one of the NVR profiles
- Manually install NVR and drag it to the "Optional NVR" Separator.
- Place the mod at the top of the NVR separator so that all the NVR mods below it that you enable will overwrite the mod files.
3. Enable either **Hikikomori NVR** or **Caffiene NVR**, your preference.
  - There are a few performace mods for Caffeiene NVR

### 🔧 Shader Package

This mod is optional but it does fix directional reflections in your game, I recommend it.

1. Navigate to:  
Documents\My Games\FalloutNV
2. Open `RendererInfo.txt`
3. Find your **shader model** (2nd line from bottom)
4. Go into **MO2** and locate your shader package number in the **shader package separator** under **Optionals**
5. Enable the box and that's it.

---

### 🕹 In-Game
1. Complete the intro with Doc. DO NOT LEAVE THE HOUSE.
2. Go to the MCM. ESC > M.
3. Find Quickthrow. Toggle the box to disable the name.
4. Save and exit the game. Reload your save.
5. UI should not overlap and the pip boy real time map should be working.

---

## 🔄 Updating the Modlist

To update:

1. Re-download the Wabbajack file — it will update automatically

2. For any manually added mods:
- Add `[NoDelete]` to their names

3. Add `[NoDelete]` to:
- Vanilla UI Extension
- New Vegas Reloaded
- Shader Package #
- Cyberware

---

## 🎮 Running the Game

There are **5 profiles**:

- **Normal:** 2K textures
- **Performance:** 2k textures cut in half with 1k textures where found
- **Hardcore:** Same as Normal + extra hardcore mods
- **Normal NVR** 2k textures with NVR mods enabled (still need to enable a preset)
- **Hardcore NVR** Same as Normal + extra hardcore + NVR mods (still need to enable a preset)

> 🔹 To play, make sure **New Vegas** is selected in the MO2 drop down
>  
> ❌ Do **NOT** use Fallout Launcher or NVSE directly

- Fallout Launcher will appear the **first time** — that's okay
- Missing profile-specific game INI files — that's okay
  - Click OK and continue
- Close it and relaunch the game via MO2

---

## 🎮 Hotkeys - K in pause menu to view. Use Keybinder MCM to configure to your preferences and set up.

### 🧭 In-Game Menu Shortcuts
| Key                           | Action                       |
| ----------------------------- | ---------------------------- |
| `ESC`                         | Pause Menu                   |
| `N`                           | Menu Overhauls               |
| `M`                           | Mod Configuration Menu (MCM) |
| `T`                           | Achievements Menu            |
| 🔼 *(Up Arrow, bottom right)* | HUD Editor                   |

### ⌨️ Keyboard Controls
| Key / Combo     | Action                                     |
| --------------- | ------------------------------------------ |
| `WASD`          | Move                                       |
| `E`             | Activate / Interact                        |
| `Tab`           | Open Pip-Boy                               |
| `R`             | Ready / Reload weapon                      |
| `L-Ctrl`        | Sneak *(Hold to Prone)*                    |
| `L-Shift`       | Sprint                                     |
| `L-Alt`         | Hold Breath                                |
| `Caps Lock`     | Toggle Always Run                          |
| `Q`             | Toggle Always Move                         |
| `Space`         | Jump                                       |
| `F`             | Change View (1st/3rd Person)               |
| `T`             | Wait                                       |
| `V`             | V.A.T.S.                                   |
| `J`             | Toggle Quest Log                           |
| `G`             | Throw Grenade *(B42 Quickthrow)*           |
| `H`             | Select Grenade                             |
| `R`             | Stop Grenade Throw                         |
| `O`             | Ammo Check                                 |
| `P`             | Weapon Condition Check                     |
| `X` + `Q` / `E` | Lean Left / Right While Aiming             |
| `Hold 1`        | JIP Follower Commands                      |
| `2`             | Follower Wait *(Hold to make them follow)* |
| `3`             | Real Time Pip Boy Map (Toggle)             |

### 🖱️ Mouse
| Button           | Action      |
| ---------------- | ----------- |
| `Mouse Button 4` | Bullet Time |
| `Mouse Button 3` | Weapon Wheel |

---
## 🌵 Modlist Overview

Here I will go over important parts of the modlist to help you better understand this list! 
Using **Wabbajack**, the list provides a streamlined installation process along with modern visual upgrades, gameplay refinements, and quality-of-life improvements — all while preserving the spirit and tone of New Vegas.

### ✨ Features
- **Plug-and-play installation** through Wabbajack  
- **Updated visuals** I include top of the line visual overhauls that make the mojave beautiful, but dangerous. There are so many visual upgrades but here I want to highlight some notable ones.
  -  Under **Early Loaders** are the visual baseline mods that I have built the list off of. Under **Visuals** you'll see a majority of the visual upgrades. I followed the SALVO guide for downloading the best retextures on the Nexus so in theory you could finish the rest of the guide by compression and packaging all the restuxtures to make the game run better. But hey, that's justa theory. This list also offers NVR as an optional visual upgrade with shadows, tonemapping, increase LOD range, parrallax, and more.
- **User Interface** I've spent the majority of my time modifing the UI. It's clean, consistent, colorful where it needs to be, more detailed with widgets, icons, enemy health and boss bars. I hope you enjoy the UI as much as I do.
- **Gameplay enhancements** Gameplay for this list has changed a lot, but the core is that same. Fun and challenging. This isn't a hardcore list, but it's a list that will challenge you and keep you on your toes.
    - Enemies are de-leveled
    - Ghouls are tougher and cause radiation damage
    - NPC's will feel real, they'll be able to pick up weapons much quicker, react to situations faster, use cover MUCH more, prone, use chems, sprint, react to gunshots, and work as a team to take you down
    - Damage is redone with damage and health scaling, reworking the DT and DR mechanics to make armor truly matter
    - No more bullet sponges or meaningless protection
    - Loot is more scarce with Famine
    - Just Assorted Mods adds a weapon wheel for quick weapon selection, bullet time, dynamic crosshair, visual objectives
    - More implants with Cyberware 2281
- **Content** I've also added some new content here and there but not a lot.
    - A World of Pain Revised adds more locations to explore and quests in an immersive way
    - Dry Wells - A legion expansion
    - Long 15 - NCR expansion
    - Living Desert makes the Mojave feel more alive with more NPC's and scripted events along your travels
    - Many location overhauls that I personally like and patched to work together
    - Lucky 38 Suite Overhaul (my own creation)
- **Animations** Movement feels smoother and your character feels more alive

### 🧭 Philosophy
The goal of **High and Dry** is to provide a **stable, lore-friendly, and atmospheric** experience that feels like a remastered New Vegas without compromising what makes the game iconic.  
Every mod is chosen and tested with an emphasis on **compatibility, performance, and consistency** to ensure a smooth, crash-free playthrough.
This is all starts with Viva New Vegas. A modlist that is now an essential and highly regarded in the FNV community *Shoutout to ModdlingLinked*. 

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
