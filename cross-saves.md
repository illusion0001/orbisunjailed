---
title: "PS4 - PS Vita Cross-Saves"
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

## What are cross-saves?

* Cross-saves refer to saves that are compatible on 2 or more systems that can be used interchangeably. 
* This guide will cover PS4 to PS Vita saves and vice versa.

## Enough talk, let's start...

### Requirements

* Both PS4 & PS Vita need to be hacked/jailbroken. Firmware doesn't matter, game versions don't matter either.
* For PS4: [Apollo Save Tool](apollo-save-tool.md)
* For PS Vita: VitaShell
* Games need to follow the same or similar structure on both platforms (PS4 / Vita).

### Copying and replacing saves

* Open Apollo Save Tool > HDD Saves > Your game.
* Export Decrypted Save Files and select your USB drive.
* Apollo will create a folder on the USB drive (PS4 > APOLLO). The save file should be called SYSTEM.DAT.
* Simply rename SYSTEM.DAT to system.bin **(make sure you do rename the extension dat to bin and not system.bin.dat)**.
* Some games might have different naming schemes for the files but as long as both the Vita and PS4 have similar naming schemes then the games will most likely work.
* Copy the save to your Vita (any folder).
* On PS Vita make sure you open the game and wait until it makes a save. You need a save to be created so it can be replaced.
* Open VitaShell and navigate to ux0 > user > 00 > savedata.
* Once you see your game ID, press Triangle button > Open decrypted.
* Copy and replace system.bin.
* Done.

### Final notes

* Note that "Checking DLC content" will show again on your Vita. A bit annoying if you have all of them, you will have to spam X. This is only a first time issue tho.
* Tested and confirmed working on Persona Dancing series (3, 4 & 5) & Gundam Breaker 3 Break Edition,
* To do the same but from Vita to PS4, just follow the tutorial but backwards.
