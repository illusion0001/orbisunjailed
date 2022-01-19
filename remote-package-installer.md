---
title: "Remote Package Installer"
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

## What is Remote Package Installer and why would I use it?

 * Remote Package Installer is a homebrew application that will allow sending your packages from your PC to the PS4 without the need to use USB drives.
 * With the use of this application, you can replicate Sony's way of download and installing packages, acting the same way (downloading, installing, unpacking, etc).

### Installing and setting up Remote Package Installer

 * Remote Package Installer can be downloaded and installed via [Homebrew Store](hb-store.md).
 * After installing, open it and **keep it open, do not minimize it or go to your homescreen**. The app will just show the splash screen.
 * Download and install/unpack:
    * [PS4 PKG Sender](/backupfiles/Ps4 Pkg Sender V1.07.rar)
    * <a href="https://www.microsoft.com/en-nz/download/details.aspx?id=48130"> .NET Framework 4.6 </a>
    * <a href="https://nodejs.org/en/"> Node.js </a>
 * After installing everything, open cmd and paste the following command: **npm install http-server -g**
 * In cmd paste the following command: **ipconfig**. In IPv4 section, take note of IP Address.
 * Open PS4 PKG Sender. Server IP is your PC's IP Address. Input your PS4 IP in PS4 IP section.
 * Drag and drop your packages into the program.
 * Select Start Queue. Your packages will start to be sent to the PS4.
 * Done.

### Improving the speed of Remote Package Installer

 * For the best connection possible, use ethernet cable connection.
 * For computers or laptops with a Wi-Fi adapter and a ethernet port, you can connect a ethernet cable directly from the PS4 to the PC. On your PC open Control Panel > Network and Internet > Network and Sharing Center > Change Adapter settings > Right-click your Wi-Fi adapter > Proprieties > Sharing tab > Check Allow other networks to connect through this computer's internet connection. For those who have a drop-down menu, select Ethernet. Select OK.
