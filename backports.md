---
title: "Backports"
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

## What is a backport and do I need it?

* As you might've noticed, there are plenty of firmwares exploited in order to jailbreak. Lower firmwares, even though they are usually notorious for great stability and success rates, are technically released before newer games. Ex: 5.05 firmware was released back in 2018 while a game like Persona 5 Strikers was released in 2020.
* Sony implemented a check to force the user to update to the latest firmware in order to play newer games (both on digital versions of games and disc games). 
* Clever hackers found a way to disable that check so that no matter what firmware version you have and how old it might be, the game/app could be launched. That kind of patch is called a backport patch.
* Do I need a backport patch? Yes and no. It depends on your firmware. If you are on latest exploitable FW you don't need a backport until a jailbreak for a new firmware will be released (and you decide to stay on your current firmware).
* If you are on a lower firmware you will need a backport patch in order to launch a newer game. Here you can find out what game requries which firmware:
<a href="https://oldnero.github.io/PS4-Games-List/"> PS4 FW Game List </a>

## Enough talk, let's start...

* Make sure you have your games and updates extracted, everything should be .pkg files.
* Download and extract AutoBackPort Tool:
[AutoBackPortv1.11](/backupfiles/AutoBackPort_1.11.rar)

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
