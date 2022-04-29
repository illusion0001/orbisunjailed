---
title: "FPS Patches & Mods"
mathjax: true
layout: post
categories:
  - info

# Menu

navigation:                # accepts {file, title, url, icon, sidebaricon}
  - {file: "home.md", title: "Home"}
  - {file: "about-general-knowledge.md", title: "About & General Knowledge"}
  - {file: "Jailbreak.md", title: "Jailbreak"}
  - {file: "gaming.md", title: "Games, Updates & DLC"}
  - {file: "hacks-homebrew.md", title: "Hacks & Homebrew"}
---

## What mods can I install and how do 60FPS patches work?

* While PS4 mods are not as popular as some other platforms like PSVita, PS3, there are some mods you can do to your games than can range from character model swaps, music swaps, etc.
* FPS patches work by modifying some lines from the game's main executable (eboot.bin) that will toggle FPS unlock by sacrificing resolution. Basically higher FPS will need lower resolution.
* Here is a list of all 60FPS patches available:
<a href="https://illusion0001.com/patch/"> PS4 60FPS & Resolution Patch List </a>

## Enough talk, let's start...

### 60FPS & Resolution Patches

* Download and extract/install the following tools:
    * <a href="https://anonfiles.com/n411Q0Bfxd/Patch_Builder_v1.3.2_zip"> PS4 Patch Builder v.1.3.2 </a>
    * <a href="https://github.com/illusion0001/py-patcher-bin"> Py-Patcher </a>
* Dump the update of a game by launching the game and keeping it running. Via FTP dump patch (ac) in /mnt/sandbox/pfsmnt/.
* Open py-patcher. Select Y to download patch0.
* Drag and drop eboot.bin to the cmd window.
* Select the appropriate patch. Wait.
* A new eboot.bin will appear in eboot.bin-patched folder in pypatch directory. Replace old with new.
* Open PS4 Patch Builder, select Image 0 on Project Location by dragging and dropping. For Package Settings drag and drop the original game .pkg.
* On Patch Notes you can add text like "60FPS mode". **Make sure to pick a different version than it is (ex: if patch is 01.01, change to 01.011)**
* Select output and build.
* Copy the finished pkg to the root of a USB drive.
* Navigate to Settings > GoldHEN > Package Installer and install the game, updates, dlc (if you don't have them installed already) then the fake update that contains the patch.
* Done.


### Other mods

 * These mods are the scarce ones, that are already built as pkg to install. As a result I will only provide links to some mods I found:
    * <a href="https://www.psx-place.com/forums/ps4-game-mods.226/"> PS4 Game Mods Subforum </a>
    * <a href="https://www.psxhax.com/threads/mortal-kombat-xl-modpack-2-for-ps4-4-user-friendly-players.5121/"> Mortal Kombat XL Modpack </a>
    * <a href="https://old.reddit.com/r/ps4homebrew/comments/qx78u8/resident_evil_2_classic_modpack/"> Resident Evil 2 Classic Modpack </a>
    * <a href="https://old.reddit.com/r/ps4homebrew/comments/quxe28/resident_evil_3_classic_modpack/"> Resident Evil 3 Classic Modpack </a>
