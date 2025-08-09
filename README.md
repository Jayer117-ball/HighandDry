
![Banner Readme](https://github.com/user-attachments/assets/cd44d8cf-4901-48e6-9577-daa3a7deb2fc)

# High and Dry Modlist Installation Guide

Welcome! This guide will help you install my **Fallout: New Vegas** modlist using **Wabbajack**. Whether you’re new to modding or just need some extra guidance, follow these steps carefully, and you’ll be playing a fully modded New Vegas in no time!

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
- Read the **Introduction** and **Setup** pages from the [Viva New Vegas Guide](https://vivanewvegas.moddinglinked.com/intro.html)
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

## 📦 Post-Installation Steps

### 🔁 Run 4GB Patch

1. Open **Mod Organizer 2** that shipped with High and Dry
2. Click the Executable drop down and click on **FNVPatch**
- Check to see if the Binary path is correct before running the patcher
- https://github.com/Jayer117-ball/HighandDry/blob/main/4GB%20Patch.png
4. MO2 will load the application
5. After running `FNVpatch` — it should confirm:  
   `FalloutNV.exe patched!`

### 📜 Install Vanilla UI Extension

1. Download [Vanilla UI Extension](https://www.moddb.com/mods/vanilla-ui-extension/downloads/vanilla-ui-extension-10)
2. Install it manually through **Mod Organizer 2**
3. Place it **after Vanilla UI Plus** in the left pane

### ⚙️ DXVK or Heap Replacer (Choose One)

- **Default (Recommended):** DXVK 2.7
- **Alternative:** New Vegas Heap Replacer. Older, not up to date

> ⚠️ **Only use one**, not both

---

## 🚀 First-Time Launch

- Launch **Fallout: New Vegas through Steam** once to generate config files
- Let it detect your resolution, then close it
- Always launch the game via **Mod Organizer 2**

---

## 📝 Notes

- Expand the **separators in MO2** and read notes on individual mods. Most notes can be expanded for more information.
- Some mods have extra features or useful usage tips

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

---

## ⚙️ Optional Steps

### 🧃 BSA Decompressor

- Go to your installation folder
- Run `FNV BSA Decompressor.exe`  
→ Reduces load times and stutters

### 🌃 New Vegas Reloaded (NVR)

1. Download the **latest Nightly Build** from [TES Reloaded Discord](https://discord.com/invite/BYY7SNfQeJ)
2. In MO2:
- Set NVR load order:
  - **823** = Normal/HC
  - **545** = Performance
- Enable:
  - Cartographer
  - NVR - Lucky 38 Shadows Fix
  - High and Dry NVR Main Menu Replacer
  - Desert Natural Weathers + Performance + Dry Wells Patch
  - Neutral Weathers
  - Caffeine NVR + Performance + RTR
  - Sundry NVR Fixes Reloaded 2
  - SFX NVR Pack
  - Special Series – Fire Barrel FX
  - NVR versions of:
    - Lucky 38 Exterior Remastered
    - Strip Cinematic Lighting Overhaul

- Disable:
  - Weathers Revised + Weather Variation + the Lucky 38 Lights Redone patch (located in the **Weather Visuals** separator)
  - 3D Rain + patches
  - High Resolution Bloom
  - Non-NVR versions of the mods of:
    - Lucky 38 Exterior Remastered
    - Strip Cinematic Lighting Overhaul

### 🔧 Shader Package

This mod is optional but it does fix directional reflctions in your game, I recommend it.

1. Navigate to:  
Documents\My Games\FalloutNV
2. Open `RendererInfo.txt`
3. Find your **shader model** (2nd line from bottom)
4. Download the correct [shader package](https://www.nexusmods.com/newvegas/mods/69135) based on your model
5. Install it into MO2 like any other mod

---

## 🎮 Running the Game

There are **3 profiles**:

- **Normal:** 2K textures
- **Performance:** 1K textures
- **Hardcore:** Same as Normal + extra hardcore mods

> 🔹 Run the game through **MO2**
>  
> ❌ Do **NOT** use Fallout Launcher or NVSE directly

- Fallout Launcher will appear the **first time** — that's okay
- Close it and relaunch the game via MO2

---

## 🎮 Hotkeys - K in pause menu to view

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

### 🖱️ Mouse
| Button           | Action      |
| ---------------- | ----------- |
| `Mouse Button 3` | Bullet Time |

---

## 🆘 Need Help?

- **Game won’t launch?**  
Make sure you have the **latest VC++ Redistributables**

- **Still won’t launch?**  
Make sure you copied **Root Mods** correctly

- **Still still won’t launch?**  
Make sure the **4GB patch** was applied!

- **Still still still won’t launch?**  
Don’t install FNV to `Program Files` — [learn how to change it](https://vivanewvegas.moddinglinked.com/setup.html)

- **Still still still STILL won’t launch?**  
Hey, it happens! Join the [Discord](https://discord.gg/zV5zACunk3), read the FAQ, and ask in the correct channel

---
