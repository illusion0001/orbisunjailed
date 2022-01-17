---
title: "app.db Tweaks"
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

## What is app.db and what can I do with it?

* app.db is the file that holds a database of every single app / game installed on the PS4.
* By editing the file, you can hide system apps that are just wasting space or are useless on a jailbroken PS4 such as News, PS Store, PLAYROOM, etc.

## Enough talk, let's start...

* Download and install:
       * <a href="https://sqlitebrowser.org/dl/"> SQLite Browser </a>
       * <a href="https://filezilla-project.org/download.php?type=client"> FileZilla FTP </a>
 * Jailbreak using GoldHEN.
 * Navigate to Settings > GoldHEN > Enable FTP. Take note of the IP Address.
 * Open FileZilla and input PS4's IP Address on host and 2121 on port.
 * FileZilla > Server > Enter custom command > MTRW (must be all caps).
 * Navigate to /system_data/priv/mms and copy app.db to Desktop.
 * Open SQLite Browser and open app.db
 * A list of all the apps will show. To hide a app, simply scroll right until you see **isVisible**. Input value 0 to hide or 1 to unhide.
 * Save the file.
 * Back to Filezilla simply replace app.db with the edited one.
 * Reboot your PS4.
 * Done.
