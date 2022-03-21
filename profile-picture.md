---
title: "Customizing Profile/Avatar"
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

## How can I customize my avatar?

* Profile picture is the profile icon found in the various parts of the OS, such as homescreen (function area), quick menu, log-in screen, etc.
* This guide will show you how you can easily make any picture as the profile avatar and how to change your account name.
* **Note that you need a activated account first!**

## Changing avatar picture

* Download and install:
     * <a href="https://mega.nz/file/zs5GUCjT#BGEh3sAYpyFwxFM6dXVYS2j1jTwlcb2y70XenWOl2oU"> PS4 Avatar Maker by Lappy </a>
     * <a href="https://pkg-zone.com/details/LAPY20001"> PS4 Xplorer by Lappy </a>
     * <a href="https://directx-9-0c.en.lo4d.com/windows"> DirectX 9.0 needed for PS4 Avatar Maker </a>
* After installing everything, including DirectX 9.0, prepare your image (format doesn't matter).
* Make sure your image is a perfect square format, to ensure no part of the image will be cropped or stretched (use any type of image editor if needed).
* Open PS4 Avatar Maker, select the type of account (Local or Activated).
* Double click the middle part and select your image.
* Select Export Avatar, and select a name and location.
* Put the exported avatar on a USB Drive or FTP to a location on the internal HDD of the PS4.
* On the PS4, jailbreak using GoldHEN.
* Open PS4Xplorer, navigate the location of the avatar you set.
* Select it and press X to apply (you might need to do it 2 times).
* To see it, log out and log back in your account (you don't need to reboot).
* Done.

## Changing profile name

* Jailbreak your PS4 with GoldHEN.
* Navigate to PS4 > GoldHEN > Enable FTP server. Take note of PS4's IP Address.
* On PC, open FileZilla or your desired FTP client and input the PS4's IP as host and port 2121.
* Navigate to **/system_data/priv/cache/profile/0xNUMBERSYOUHAVE**.
* Edit online.json on Notepad++ or any text editor. If you don't have a online.json, <a href="https://gbatemp.net/attachments/0x10000009-generic-rar.220121/"> download a copy here </a>
* Replace "myFirstName" with your desired name.
* Replace "myLastName" with your desired name. **If you don't want a last name, leave the section as "".**
* Save changes and replace online.json with old one.
* Done.
