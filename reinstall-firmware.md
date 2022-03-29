---
title: "Reinstalling Firmware"
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

## Why should I reinstall my firmware and how can I?

* Reinstalling the firmware is a possibility jailbroken users can do **(with and without removing data)** if you have issues with your PS4 **(should be last option)** or used homebrew applications and tweaks that require it for a complete removal *(such as ReSys Flasher)*.
* This guide will provide both methods to achieve the reinstall with and without data loss.

## Reinstalling firmware WITHOUT losing data

* **This will keep all data including games, save data.**
* Download 9.00 (or your current) firmware file on your PC by visiting one of the sites **(do not get full/recovery firmwares - get update firmware)**
   * <a href="https://darksoftware.xyz/PS4/FWlist">DKS - PS4 Official Firmwares (darksoftware.xyz)</a> Recommended because of the faster download speeds but requires creation of an account on the site.
   * <a href="https://darthsternie.net/ps4-firmwares/">PS4 Firmwares - Darthsternie's Firmware Archive</a> No account required, but slower download speeds.
* Unpack your archive and rename the file to **PS4UPDATE.pup** (must be in all caps).
* Prepare a USB stick drive by formatting it to **FAT32** and creating a folder on the root of the drive named **PS4** and another folder inside PS4 named **UPDATE**. Copy PS4UPDATE.pup in the UPDATE folder.
* Final structure should look like this: **PS4 > UPDATE > PS4UPDATE.pup**
* Boot into PS4's recovery settings by turning off the PS4 and holding the PS4 button until it beeps 2 times. Recovery mode should look like this:

![Recovery mode](/images/safemode.jpg)

* Plug the USB stick into an empty slot on your PS4.
* Select 3. Update System Software > 1. Update from USB Storage Device > OK > Update.
* The PS4 will now install the firmware and remove everything on the HDD.
* **REMOVE ANY ETHERNET CABLE AND/OR SKIP WI-FI SETUP. Keep everything offline during and after setting up your PS4.**
* **After setup, navigate to Settings > System > Automatic Downloads > Uncheck Featured Content, System Software Update Files, Allow Restart and Application Update Files.**
* Done.  
 
## Reinstalling firmware and starting fresh

* **This will NOT keep all data including games, save data.**
* Download 9.00 (or your current) firmware file on your PC by visiting one of the sites **(do not get beta firmwares - get recovery/full firmwares - should be over 1GB file size depending on the version)**
   * <a href="https://darksoftware.xyz/PS4/FWlist">DKS - PS4 Official Firmwares (darksoftware.xyz)</a> Recommended because of the faster download speeds but requires creation of an account on the site.
   * <a href="https://darthsternie.net/ps4-firmwares/">PS4 Firmwares - Darthsternie's Firmware Archive</a> No account required, but slower download speeds.
* Unpack your archive and rename the file to **PS4UPDATE.pup** (must be in all caps).
* Prepare a USB stick drive by formatting it to **FAT32** and creating a folder on the root of the drive named **PS4** and another folder inside PS4 named **UPDATE**. Copy PS4UPDATE.pup in the UPDATE folder.
* Final structure should look like this: **PS4 > UPDATE > PS4UPDATE.pup**
* Boot into PS4's recovery settings by turning off the PS4 and holding the PS4 button until it beeps 2 times. Recovery mode should look like this:

![Recovery mode](/images/safemode.jpg)

* Plug the USB stick into an empty slot on your PS4.
* Select 7. Initialize PS4 (Reinstall System Software) > OK > Yes.
* The PS4 will now install the firmware and remove everything on the HDD.
* **REMOVE ANY ETHERNET CABLE AND/OR SKIP WI-FI SETUP. Keep everything offline during and after setting up your PS4.**
* **After setup, navigate to Settings > System > Automatic Downloads > Uncheck Featured Content, System Software Update Files, Allow Restart and Application Update Files.**
* Done.  
