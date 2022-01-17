---
title: "Remote Play"
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

## PC-PS4 Remote Play

### Using patched Remote Play client
 * Note that you will need a PSN account (can be a dummy one and never connected/linked to the PS4).
 * Download and extract the following tools:
[Patch Remote Play Client - must be this version](/backupfiles/PS4 Remote Play 2.6.0.2270.zip)
[Remote Play Patcher](/backupfiles/PS4.Remote.Play.Auto-Patcher.zip)

 * Install the patched client. Note: in latest version of Win10 if you get Media Pack error navigate to Settings > Apps > Apps & features > Optional features and remove and install again Windows Media Player.
 * Open Remote Play Patcher and patch it. Note: Windows Defender might block the program. Disable it, file is trusted by PS4 Homebrew community.
 * After jailbreaking your PS4 using GoldHEN navigate to Settings > Remote Play Connection Settings > Enable Remote Play and Remote Play using PSVita/PSTV.
 * Select Add Device and take note of the code.
 * Back to the PC, open Remote Play application, connect to PS4 and sign-in to your dummy PSN account.
 * Select register manually and enter the code.
 * Done.

## PSVita-PS4 Remote Play



**For games without updates:
 * Open AutoBackport, set Base Game as the game's .pkg file and set Destination folder to a output folder.
 * Build backported pkg file for the base game. (The result will be a small sized pkg file acting as a fake update)
 * Add the main game pkg and the fake update pkg to the root of a USB drive.
 * Plug the drive to the PS4.
 * Navigate to the PS4 > Settings > GoldHEN > Package Installer and install main game pkg first then the fake update pkg.
 * Done.

**For games with updates:
 * Open AutoBackport, set Base Game as the game's .pkg file, set Update PKG to the .pkg file and set Destination folder to a output folder.
 * Add the main game pkg, update pkg and the fake update pkg to the root of a USB drive.
 * Plug the drive to the PS4.
 * Navigate to the PS4 > Settings > GoldHEN > Package Installer and install main game pkg first, update pkg second then fake update pkg.
 * Done.


## Troubleshooting

 * I installed everything and I get error CE-40740-5. This could be a result of multiple things. Check your PC folder's permissions, available disk space & check and disable AntiVirus if it detected a false postivie. The tool is trusted and completely safe by the PS4 Homebrew community.
