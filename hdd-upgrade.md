---
title: "Upgrading PS4's Internal HDD"
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

## How can I upgrade PS4's HDD?

* **This guide will provide how to safely upgrade or replace your PS4's Internal HDD without updating your firmware or losing data.**
* This guide does not apply to external HDDs as they are seen and act differently on PS4.
* **If you DON'T want to keep any data but still wish to upgrade your HDD, scroll down to the last section.**

## Upgrading/replacing HDD with a HDD of same size
* This is the recommended way to replace your HDD **only if both HDDs are the same size**.
* Look at the other method, for bigger or smaller HDDs.
* You will need a HDD enclosure or another way to connect the old and new HDD to a PC and a small USB drive (4GB minimum).
* Download and extract your firmware **you are currently on. Download recovery firmware**.
   * <a href="https://archive.midnightchannel.net/SonyPS/Firmware/index.php?cat=PS4SYS">Midnight Channel Archives</a> - Recommended because of the faster download speeds.
   * <a href="https://darksoftware.xyz/PS4/FWlist">DKS - PS4 Official Firmwares (darksoftware.xyz)</a> Recommended because of the faster download speeds but requires creation of an account on the site.
   * <a href="https://darthsternie.net/ps4-firmwares/">PS4 Firmwares - Darthsternie's Firmware Archive</a> No account required, but slower download speeds.
* **Do not try to download a firmware lower than your current as it will NOT install. Also, do not try to download a higher firmware as it will update your PS4 and you WON'T be able to downgrade**
* Format the USB drive as FAT32 or exFAT and create the following structure: PS4 > UPDATE > PS4UPDATE.pup *(rename the pup to PS4UPDATE.pup if you didn't already)*
* Take your original HDD out of PS4. Insert the new HDD inside. Plug-in the USB Drive to the PS4.
* Hold PS4's power button (button on the console, not the controller) until you boot into Safe Mode.
* Initialize PS4 using the USB Drive. **Make sure the firmware is the same as your original HDD. Do NOT initialize if firmware is higher or lower!**
* Wait until it's done and finish setting up your PS4.
* **REMOVE ANY ETHERNET CABLE AND/OR SKIP WI-FI SETUP. Keep everything offline during and after setting up your PS4.**
* **After setup, navigate to Settings > System > Automatic Downloads > Uncheck Featured Content, System Software Update Files, Allow Restart and Application Update Files.**
* Put the original HDD into the Hard Drive enclosure and plug-it in your PC.
* Download and install:
   * <a href="http://hddguru.com/software/HDD-Raw-Copy-Tool/"> HDD Raw Copy Tool </a> If you're using Windows!
   * <a href="https://bombich.com/"> Carbon Copy Cloner 6 </a> If you're using MacOS!
* **Make a FULL backup of your drive. DO NOT SKIP ANY FILE. It must a complete full backup!**
* Wait, it will take a while depending on the size of the drive.
* After the backup has been done, remove the new HDD from your PS4 and insert it on your Hard Drive Enclosure and plug-it back to your PC.
* Open the same program as before and restore the backed up image created previously on the new HDD.
* Wait, it will take a while.
* Plug the HDD back on your PS4, and power on your PS4.
* Done.


## Upgrading/replacing HDD with a bigger/smaller HDD
* This is the recommended way to replace your HDD **to a bigger or smaller HDD**.
* **This method is the official way made directly by Sony that will keep Games and apps, Saved data, Screenshots and video clips & Settings**
* Why can't we use the same way as before? Cloning the HDD to a bigger HDD will not reflect the new HDD space (ex: cloning a 500GB HDD to a 1TB HDD will make it another 500GB drive, the rest are lost).
* You will need a external HDD as big as the original HDD, a USB drive.
* You will also need a activated account.
* Plug in the external HDD to the PC and format it as exFAT.
* Plug it back to your PS4.
* Navigate to Settings > System > Back Up and Restore.
* Select Backup. Choose everything you want to keep (You must keep Saved data & Settings at the very least). **Note!: It will NOT save trophies!**
* Add a name and select Backup.
* Wait, it will take a while, depending on what you choose.

### Backing up Trophies
* **If you do not wish to backup your trophies, skip this fix. Skipping this step will NOT cause any issues.**
* On your PS4, open Internet Browser and visit the following host: https://kar0218.github.io/
* Select your firmware.
* Plug in a USB drive formatted as exFAT.
* Select DB Backup function.
* Wait, have patience.

### Continuing the guide
* Download and extract your firmware **you are currently on. Download recovery firmware**.
   * <a href="https://archive.midnightchannel.net/SonyPS/Firmware/?cat=ps4rec">Midnight Channel Archives</a> - Recommended because of the faster download speeds.
   * <a href="https://darksoftware.xyz/PS4/FWlist">DKS - PS4 Official Firmwares (darksoftware.xyz)</a> Recommended because of the faster download speeds but requires creation of an account on the site.
   * <a href="https://darthsternie.net/ps4-firmwares/">PS4 Firmwares - Darthsternie's Firmware Archive</a> No account required, but slower download speeds.
* **Do not try to download a firmware lower than your current as it will NOT install. Also, do not try to download a higher firmware as it will update your PS4 and you WON'T be able to downgrade**
* Format the USB drive as FAT32 or exFAT and create the following structure: PS4 > UPDATE > PS4UPDATE.pup *(rename the pup to PS4UPDATE.pup if you didn't already)*
* Remove external HDD. Take your original HDD out of PS4. Insert the new HDD inside. Plug-in the USB Drive to the PS4.
* Hold PS4's power button (button on the console, not the controller) until you boot into Safe Mode.
* Initialize PS4 using the USB Drive. **Make sure the firmware is the same as your original HDD. Do NOT initialize if firmware is higher or lower!**
* Wait until it's done and finish setting up your PS4.
* **REMOVE ANY ETHERNET CABLE AND/OR SKIP WI-FI SETUP. Keep everything offline during and after setting up your PS4.**
* **After setup, navigate to Settings > System > Automatic Downloads > Uncheck Featured Content, System Software Update Files, Allow Restart and Application Update Files.**
* Jailbreak your PS4 using GoldHEN.
* Insert the external HDD you used to make a backup.
* Go to Settings > System > Back Up and Restore.
* Select Restore PS4. Select the backup. Press Yes to restore.
* Wait until it restores, it may take a while. Have patience.
* After you have sucessfully restored, jailbreak your PS4 using GoldHEN. Test a game or too.
* Done.

### Restoring Trophies
* **In case you chose earlier to backup your trophies, this continues the guide by restoring them safely back to your PS4.**
* On your PS4, open Internet Browser and visit the following host: https://kar0218.github.io/
* Select your firmware.
* Plug in the USB drive you saved the files earlier.
* Select DB Restore function.
* Wait, have patience.
* Done.


## Upgrading/replacing HDD WITHOUT keeping any data
* **Do NOT do this section if you DO wish to keep your data! If you want to keep your data follow one of 2 sections above to your use case!**
* Download and extract your firmware **you are currently on. Download recovery firmware**.
   * <a href="https://archive.midnightchannel.net/SonyPS/Firmware/index.php?cat=PS4SYS">Midnight Channel Archives</a> - Recommended because of the faster download speeds.
   * <a href="https://darksoftware.xyz/PS4/FWlist">DKS - PS4 Official Firmwares (darksoftware.xyz)</a> Recommended because of the faster download speeds but requires creation of an account on the site.
   * <a href="https://darthsternie.net/ps4-firmwares/">PS4 Firmwares - Darthsternie's Firmware Archive</a> No account required, but slower download speeds.
* **Do not try to download a firmware lower than your current as it will NOT install. Also, do not try to download a higher firmware as it will update your PS4 and you WON'T be able to downgrade**
* Format the USB drive as FAT32 or exFAT and create the following structure: PS4 > UPDATE > PS4UPDATE.pup *(rename the pup to PS4UPDATE.pup if you didn't already)*
* Take your original HDD out of PS4. Insert the new HDD inside. Plug-in the USB Drive to the PS4.
* Hold PS4's power button (button on the console, not the controller) until you boot into Safe Mode.
* Initialize PS4 using the USB Drive. **Make sure the firmware is the same as your original HDD. Do NOT initialize if firmware is higher or lower!**
* Wait until it's done and finish setting up your PS4.
* **REMOVE ANY ETHERNET CABLE AND/OR SKIP WI-FI SETUP. Keep everything offline during and after setting up your PS4.**
* **After setup, navigate to Settings > System > Automatic Downloads > Uncheck Featured Content, System Software Update Files, Allow Restart and Application Update Files.**
* Jailbreak your PS4 using GoldHEN.
* Done.
