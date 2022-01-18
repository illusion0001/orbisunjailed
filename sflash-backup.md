---
title: "Backing up sflash"
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

## What is sflash and why do I need to back this file?

 * **This process will be useful for repairs and future progress to a hopeful downgrade method.**
 * Backing up sflash is very useful if you somehow manage to completely brick the console or if you load bad/corrupted payloads that will affect PS4's ability to boot.
 * **Note that if you are careful and have common sense, you won't ever kill your console, unless you're a bad thinkerer. This procedure is to keep your console safe.**

### Backing up sflash

 * Jailbreak your PS4 using GoldHEN.
 * Navigate to Settings > GoldHEN > Enable FTP Server. Take note of your PS4's IP Address from the notification.
 * On your PC, download and install:
    * <a href="https://filezilla-project.org/download.php?type=client"> FileZilla FTP Client </a>
 * Open FileZilla and on **Host name** input your PS4's IP Address you noted, on **Port** input 2121.
 * Navigate to **/dev/**. Copy sflash0 file to your PC's desktop.
 * **Make sure it's exact size after the copy is 32MB / 32768 KB / 33554432 bytes.**
 * Keep the file saved in a safe location.
 * Done.

## Backing up PS4's HDD

 * **Note that this will clone a ENTIRE PS4 HDD. Meaning you need to have at least the HDD's space for a full backup. Ex: if you have a 500GB HDD in your PS4, you need more than 500GB to make a backup on your PC.**
 * As a alternative you can install a small HDD to your PS4, install the firmware, then attempt the backup.
   * PS4 can support 160GB as the smallest HDD size.
 * After you have the PS4 on a exploitable firmware, turn off your PS4. Remove the HDD from your PS4.
 * Insert the PS4's HDD to the PC.
 * Download and install"
    * <a href="https://www.flashfxp.com/"> FlashFXP </a>
 * Open FlashFXP, select the PS4's HDD then select Continue.
 * Double click on File, select a Output folder and name it **ps4hddbackup**. Don't forget to add the firmware number to the name.
 * Select Continue. Select Start.
 * Wait and have patience. **Depending on the size of the HDD you are cloning, it can take a LONG time.**
 * Done, you can insert the HDD back on your PS4.
