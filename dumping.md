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
     * <a href="https://github.com/CyB1K/PS4-Fake-PKG-Tools-3.87/archive/refs/heads/main.zip"> FAKE PKG Tools </a>
  * Open GP4 Generator. In CUSAxxxx Dir put the directory of the -app folder on your external HDD. Ex: E:/CUSA43953-app
  * Select Generate GP4. Wait and have patience.
  * After it has been completed a "Done" should appear at the bottom. Select Save GP4 and save it on the root of the USB drive.

#### Fixing NP Errors
  * NP errors are usually realted to encrypted trophies. A quick summary, is when you don't try to fix them, when you make the fpkg and try to launch them a error will immediately appear with a random NP-xxxx code.
  * **Not all games will need this fix, but most game updates/patches will, so it's better to keep it save and see if you need this patch or not.**
  * Download and install:
     * <a href="https://mh-nexus.de/en/downloads.php?product=HxD20"> HxD Editor </a>
     * <a href="https://filezilla-project.org/download.php?type=client"> FileZilla FTP </a>
  * Open HxD and open **trophy00.trp** from your **extracted game's folder > sce_sys > trophy** AND from the **extracted patch folder > sce_sys > trophy.**
     * In the decoded text section, if you can cleary read the contents (ex: TROPHYCONF.ESM, TROP.ESM, etc), then you have a unencrypted file. In this case, you don't have to do anything.
     * In the decoded text section, if you see gibberish or scrambled text (ex: d%ns8c), then you have a encrypted file. In this case, you need to apply the fix.
  * To fix this issue you need to FTP to your PS4. Navigate on your PS4 to Settings > GoldHEN > Enable FTP Server. Take note of your PS4's IP Address from the incoming notification.
  * In FileZilla's **Host** section input your PS4's IP Address, in **Port** section input 2121.
  * Navigate to **/user/trophy/conf**. 
  * Depending on your number of installed games, you should see a bunch of folders with their own unique ID. 
  * To find out your game's ID, in your extracted game's folder (or patch if it's the one with the unencrypted file), navigate to **extracted folder > sce_sys** and open npbind.dat using HxD. In the decoded text section, your game's ID will show.
  * Back on FileZilla, open your game's ID folder and copy TROPHY.TRP file to sce_sys > trophy folder. 
  * Simply delete the encrypted one and rename the file we just copied to trophy00.trp.
  * Done.

#### Continuing on building fake pkg

  * Repeat the process if you have -patch folder and other.
  * Open orbis-pub-gen.exe.
  * Select CUSAxxx-app.gp4 made and select Build. Set the output folder and select Build again.
  * Do the same thing for the CUSAxxx-patch.gp4.
  * Done.
  * Install the pkg on your PS4 via Settings > GoldHEN > Package Installer.

### Dumping Remastered Packages

  * **Remastered packages are not refering to remastered games.**
  * Remastered packages are the type of packages that combine the main game and updates into one. This is different from usual cases where you would find one package for the main game and another for the updates.
  * The dumping process is the same as before.
  * The difference would be after inserting the HDD back to the PC, the patch folder would be empty.
  * If you try to build the fpkg, orbis-pub-gen would give a error saying that remastered packages are not supported.
  * To fix that, in the FPKG Tools folder, open orbis-pub-sfo.exe then hit File > Open.
  * Open in the extracted game's folder > sce_sys > param.sfo.
  * Once opened, simply uncheck **For the Remaster Package**. Then hit File > Save.
  * A erorr will appear, but don't worry, the changes will be still applied.
  * Done. You can continue building the fpkg using orbis-pub-gen.exe as above.
