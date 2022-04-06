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
* Download and install:
   * <a href="http://hddguru.com/software/HDD-Raw-Copy-Tool/"> HDD Raw Copy Tool </a> If you're using Windows!
   * <a href="https://bombich.com/"> Carbon Copy Cloner 6 </a> If you're using MacOS!
* **Make a FULL backup of your drive. DO NOT SKIP ANY FILE. It must a complete full backup!**
* Wait, it will take a while depending on the size of the drive.
* Done, you can insert the HDD back on your PS4.
