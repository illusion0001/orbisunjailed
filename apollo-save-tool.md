---
title: "Apollo Save Tool"
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

## What is Apollo Save Tool?
 * Apollo Save Tool is a homebrew application designed to manage save-game files. It allows to download, unlock, patch and resign save-game files directly on your PS4.
 * It also supports Save Wizard saves.
 * Apollo Save Tool can also do some other tweaks such as account unlocking and parental passcode recovery.
 * It is the preffered method because you don't need any extra work or the need of PC.


## Enough talk, let's start...

### Managing save-game files
 * Apollo Save Tool can be downloaded <a href="https://github.com/bucanero/apollo-ps4"> here </a>
 * Alternatively, it can also be found via [Homebrew Store](hb-store.md)
 * Jailbreak you PS4 using GoldHEN.

#### Online database
 * The online database is a ever growing collection of save files for PS2, PS3 & PS4 games. Users can submit their own save file <a href="https://github.com/bucanero/apollo-saves"> here </a>.
 * Simply navigate to online database section, select your game, and download to a USB drive or to internal HDD.
 * Navigate to either USB saves or HDD saves, depending on where you chose to save them.
   * If you selected HDD saves, check to see if they appear in the HDD saves section.
   * If you selected USB saves, navigate to USB saves and copy to HDD.
 * Open your game, done.

#### Copying saves between multiple profiles
 * This is useful if you have multiple accounts like User1, User2 etc.
 * Simply navigate to HDD saves, copy to USB.
 * Log in to your secondary profile.
 * Navigate to USB saves and copy to HDD.
 * Open your game, done.

#### Managing encrypted saves
 * Encrypted saves are saves made from retail/unjailbroken PS4s made via Account Data Management feature. Note, that the saves must be from 9.00 or lower.
 * On a USB drive formatted as exFAT, put the saves in the following structure : **/PS4/SAVEDATA/account-id/** *(account-id will be a section of numbers and letters, ex: 1gc30977hke0c76)
 * Back to the PS4, open the game the save was made for, and make a brand new save. **Minimize the game and keep the game running!**.
 * Open Apollo Save Tool.
 * Navigate to USB Saves. Select the save.
 * Select copy to HDD. Select yes to resign it.
 * Check to see if the save is present in HDD Saves.
 * Done.

#### Online saves
 * These kind of saves usually come from Save Wizard. **Note that Save Wizard is not needed.**
 * Saves can be found <a href="https://www.savegamefiles.com/category/ps4-savegame/"> here </a>. 
 * **NOTE!: Make sure the saves come from the same firmware or lower than your firmware in order to work.** To see that, take note of the date of the released game, the date of the uploaded save and the date your firmware was released.
 * Jailbreak your PS4 using GoldHEN, enable FTP server. Take note of your PS4's IP.
 * On your PS4, make sure to create a new save file. Simply start the game, make the save.
 * In your PC, open FileZilla. In host name input your PS4's IP and port 2121.
 * Navigate to **/user/home/yourprofileid/**. Select the appropriate CUSA ID.
 * Simply rename the files extracted from your downloaded save files to the files you need to replace. Most games have different naming schemes so make sure to replace them according to that.
 * Back to the PS4, open Apollo Save Tool. Navigate to HDD saves.
 * Select your saves then select Apply changes & Resign.
 * Open your game. You should see the same name as before, but a different size. Done.

#### Managing save files from different CUSA IDs
 * This is a fix if you want to make use of files that are for the same game but different CUSA IDs or versions (such as standard vs deluxe/GOTY editions).
 * On the game you want the save to be applied to, make a new save.
 * Open Apollo Save Tool, select HDD saves. Select your save and select Export save-game files.
 * Open PS4Xplorer, navigate to **/data/apollo/yourprofileid/** and simply rename the folder of the CUSA ID to the version of the game you need to have the game to.
 * Back to Apollo Save Tool, select HDD saves. Select your new game ID, select Import decrypted save files. Select Apply Changes & Resign.
 * Open your game. You should see the same name as before, but a different size. Done.


### Activating offline profiles
 * **Note that you cannot change the account ID to a ID you can choose.**
 * Open Apollo Save Tool, navigate to User Tools.
 * Select Activate PS4 Accounts.
 * Select your profile.
 * Done.
