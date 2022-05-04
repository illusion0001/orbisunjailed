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

### Dumping games and updates from a PS4 to a external HDD

 * **In order to dump, you must have a original PS4 game disc or have the license for digital games that came from PSN (must be able to launch and play it).**
 * Jailbreak your PS4 using GoldHEN.
 * Note that usually the save files of a original disc game and a fake converted pkg will not work, so it's recommended to dump before you make progress in your game.
 * On the PC, format a USB HDD to exFAT. Note that it needs to be at least twice bigger than the game to insure you have enough space.


### New method - Homebrew Store

 * **This is now the preffered method to dump a game, as it's everything on PS4, no payloads, no Internet Browser, and no need to manually decrypt trophies/fix NP errors.**
 * For disc games, insert the disc on your PS4 and **make sure it is installed, and not running from the disc.** Also, for disc games, make sure the disc isn't scratched, clean it before you insert it in the PS4.
 * To have the latest game patch, use [Retail Patch Installer](orbis-patch.md).
 * Download and install on your PS4:
     * <a href="https://pkg-zone.com/Store-R2.pkg"> HB Store </a>
 * Open HB Store. Make sure you have a internet connection to auto-update itself.
 * Plug-in the exfat USB Drive. **Make sure the game isn't running.**
 * Select Installed Apps. A cover flow should show.
 * Select your game. Select Dump Game. Select OK on pop-up.
 * Game should now launch, **wait for it to load, must be in main menu**.
 * Press home/PS button on your controller, go back to HB Store. The game will suspend in the background.
 * Dumping should now start, follow the progress bar and wait, have patience.
 * Done.


### Building the dumped contents into a FAKE pkg

 * Insert the HDD back to a PC. You should have a few folders, the dumper.cfg and a .complete file. You can remove the .complete file.
 * Download and extract"
     * <a href="https://github.com/CyB1K/PS4-Fake-PKG-Tools-3.87/archive/refs/heads/main.zip"> FAKE PKG Tools </a>
  * Open GP4 Generator. In CUSAxxxx Dir put the directory of the -app folder on your external HDD. Ex: E:/CUSA43953-app
  * Select Generate GP4. Wait and have patience.
  * After it has been completed a "Done" should appear at the bottom. Select Save GP4 and save it on the root of the USB drive.
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
 
### Dumping DLC

  * DLC on the PS4 comes in 2 categories: **on-disc DLC** and **extra content DLC.**
  * Extra content DLC usually come in form of map packs, extra campaign or any additional content that is **not present in the main game files**.
  * On-Disc DLC, as the name implies, already **are on the disc/main game files**.

#### Dumping Extra Content DLC

  * This type of DLC comes from PS Store. In order to dump it, you have to have the DLC installed and ready to start on your PS4.
  * Jailbreak your PS4 using GoldHEN. Navigate to Settings > GoldHEN >  Enable FTP server. Take note of your PS4's IP Address.
  * Load the game and keep it on the main menu.
  * On your PS4, open FileZilla. Input the PS4's IP Address on host name and 2121 on port.
  * Navigate to **/MNT/SANDBOX/PFSMNT/** and locate the **-ac** folder associated with your game's CUSA ID.
  * Copy all the files to your PC.
  * Open orbis-pub-sfo and create a new SFO following:
     * Core Settings > Category: PS4 Additional Content
     * Core Settings > Content ID: your games id (format: EP0123-CUSAXXXXX_YY-ZZZZZZZZZZZZZZZZ-ac)
     * Title Text > AC Title: the game's name
     * File > Save (Save to EP0123-CUSAXXXXX_YY-ZZZZZZZZZZZZZZZZ-ac/sce_sys/param.sfo)
  * Open orbis-pub-gen and create a new pkg following:
     * File > New Project > Additional Content Package With Extra Data 
     * Double click Image0 > drag and drop your DLC directory into this. Close window
     * Click Command > Project Settings > go to Package tab > set Content ID (same as: EP0123-CUSAXXXXX_YY-ZZZZZZZZZZZZZZZZ) > set Passcode and Entitlement Key to "00000000000000000000000000000000" (32 x 0's)
     * Click Command > Build Image > specify output path > click Build.
  * Install the pkg via Package Installer.
  * Done.
  
#### Dumping On-Disc DLC
  
  * Download and extract:
     * <a href="https://github.com/codemasterv/psDLC-2.1-stooged-Mogi-PPSA-gui"> psDLC </a>
  * Search your game's DLC on the PS Store on a web browser, <a href="https://store.playstation.com/en-us/product/UP0001-PPSA01491_00-DLCEXPANSION0001"> as a example </a>.
  * Take note of the address, for the example UP0001-PPSA01491_00-DLCEXPANSION0001 is the DLC name. UP = US version, EU = Europe version, JP = Japan version.
  * Launch psDLC.exe. In Manual Input tab, paste the DLC name. Select Create fpkg.
  * In the fake_dlc_pkg folder, you will see the unlocker.
  * Install the pkg via Package Installer.


### Old method, using dumper payload

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
  * Open PS4's internet browser and navigate to the following site: https://kar0218.github.io/
  * Select your firmware and select Dumper game.
  * If you see Not Enough Memory errors continue by hitting OK.
  * Once it has loaded, the dumping process has started. **Wait and have patience. Games on PS4 are huge, so it will take a long time.**
  * Once it's completed, a pop-up saying "You're all set!" should appear.

### Building the dumped contents into a FAKE pkg

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
