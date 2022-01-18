---
title: "Dumping"
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

## What is dumping and why do I need it?

* Dumping is the process of copying and decrypting every file from a game disc in order to be converted into a fake pkg, eliminating the need of the disc when launching the game.
* This process is the only way of preserving games and it is the reason one might find these dumps online.

## Enough talk, let's start...

### Dumping from a PS4 to a external HDD

 * **In order to dump, you must have a original PS4 game disc.**
 * Jailbreak your PS4 using GoldHEN.
 * Note that usually the save files of a original disc game and a fake converted pkg will not work, so it's recommended to dump before you make progress in your game.
 * On the PC, format a USB HDD to exFAT. Note that it needs to be at least twice bigger than the game to insure you have enough space.
 * Download and save the following to the root of the USB drive:
     * <a href="https://github.com/xvortex/ps4-dumper-vtx/blob/master/dumper.cfg"> dumper.cfg </a>
 * **Make sure it is saved as a .cfg file and not .txt!**
 * Open the file using notepad or notepad++
 * Default settings should be fine but edit it according to your liking.
     * split = value ; this option will tell the dumper what to dump to the USB Drive.
     * notify= value ; This option will send a notification to the PS4 every value in seconds to show you the progress. 0 = disabled.
     * shutdown = value ; This option will shutdown the console after dumping. 0 = disabled, 1 = enabled.
  * Back to the PS4 insert the USB Drive and load your game to the main menu. **Note!: keep the game ONLY on the main menu!**
  * Hit the PS button on your controller to go the homescreen and **DO NOT CLOSE THE GAME**.
  * Open PS4's internet browser and navigate to the following site: http://karo218.ir/
  * Select your firmware and select Dumper game.
  * If you see Not Enough Memory errors continue by hitting OK.
  * Once it has loaded, the dumping process has started. **Wait and have patience. Games on PS4 are huge, so it will take a long time.**
  * Once it's completed, a pop-up saying "You're all set!" should appear.

### Building the dumped game into a FAKE pkg

 * Insert the HDD back to a PC. You should have a few folders, the dumper.cfg and a .complete file. You can remove the .complete file.
 * Download and extract"
    * <a href="https://github.com/CyB1K/PS4-Fake-PKG-Tools-3.87/archive/refs/heads/main.zip" FAKE PKG Tools </a>
  * Open GP4 Generator. In CUSAxxxx Dir put the directory of the -app folder on your external HDD. Ex: E:/CUSA43953-app
  * Select Generate GP4. Wait and have patience.
  * After it has been completed a "Done" should appear at the bottom. Select Save GP4 and save it on the root of the USB drive.
  * Repeat the process if you have -patch folder and other.
  * Open orbis-pub-gen.exe.
  * Select CUSAxxx-app.gp4 made and select Build. Set the output folder and select Build again.
  * Do the same thing for the CUSAxxx-patch.gp4.
  * Done.
  * Install the pkg on your PS4 via Settings > GoldHEN > Package Installer.
