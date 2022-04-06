---
title: "Updating to latest firmware"
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

## How can I update to latest firmware and what would I lose?

* Jailbreak is not for everyone, thus why you would want to go back to retail and PSN access.
* **Note that while updating you will NOT be able to downgrade ONLY IF you made a backup of sflash, syscon, HDD AND you are good at soldering!**

## What would I lose and what can I still carry over?

* **We do NOT know what Sony might see when you update, so risk of ban is currently unknown, thus it is recommended to reinitialize and/or wipe your HDD before updating.**
* As such, no matter if you do initialize or not, **you will lose access to**:
   * Launching/opening all your fpkg games and apps.
   * Applying all your fpkg themes. If the themes are retail and have been unlocked via a unlocker only the current applied theme will stay, rest won't be able to be applied anymore (only if you don't decide to initialize).
   * All non-persistent tweaks and payloads.
   * If you initialize, trophies will also be removed. **Note that trophies unlocked via trophy unlockers are very risky, and NOT recommended if you do not wish to initialize**.
   * Access to Linux.
* However some can be carried over, such as:
   * Saves. You can carry over saves, if being backed up via save data management. **For this to work, you NEED a <a href="https://florinsdistortedvision.github.io/orbisunjailed/activate-account/"> offline activated account with SAME account ID as your PSN one </a> and to make sure your <a href="https://florinsdistortedvision.github.io/orbisunjailed/apollo-save-tool/"> games have the same CUSA ID as your owned games </a> .** For CUSA ID you can convert region in the linked guide under "Managing save files from different CUSA IDs".
   * If you do not wish to initialize, trophies. **Note that trophies unlocked via trophy unlockers are very risky, and NOT recommended if you do not wish to initialize**.
   * If you do not wish to initialize, only the current retail theme unlocked via theme unlocker.

## Updating to latest AND initializing/erasing HDD

* **Backup your saves via Save Data Management in PS4's Settings.**
* Download firmware file on your PC by visiting the following site (do not get PS4 console update file - **get PS4 console reinstallation file**)
  * <a href="https://www.playstation.com/en-us/support/hardware/ps4/system-software/"> PS4 Firmware </a>
* Prepare a USB stick drive by formatting it to FAT32 and creating a folder on the root of the drive named PS4 and another folder inside PS4 named UPDATE. Copy PS4UPDATE.pup in the UPDATE folder.
* Final structure should look like this: PS4 > UPDATE > PS4UPDATE.pup
* Boot into PS4’s recovery settings by turning off the PS4 and holding the PS4 button until it beeps 2 times.
* Plug the USB stick into an empty slot on your PS4.
* Select 7. Initialize PS4 (Reinstall System Software) > OK > Yes.
* The PS4 will now install the firmware and remove everything on the HDD.
* Done. You can now visit Sava Data Management and restore your saves if you did a backup before.

## Updating to latest WITHOUT initializing/erasing HDD

*  Download firmware file on your PC by visiting the following site (do not get PS4 console reinstallation file - **get PS4 console update file**)
  * <a href="https://www.playstation.com/en-us/support/hardware/ps4/system-software/"> PS4 Firmware </a>
* Prepare a USB stick drive by formatting it to FAT32 and creating a folder on the root of the drive named PS4 and another folder inside PS4 named UPDATE. Copy PS4UPDATE.pup in the UPDATE folder.
* Final structure should look like this: PS4 > UPDATE > PS4UPDATE.pup
* Boot into PS4’s recovery settings by turning off the PS4 and holding the PS4 button until it beeps 2 times.
* Plug the USB stick into an empty slot on your PS4.
* Select 3. Update System Software > 1. Update from USB Storage Device > OK > Update.
* The PS4 will now install the firmware while keeping everything on the HDD.
* Done.
