---
title: "Backports"
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

## What is a backport and do I need it?

* As you might've noticed, there are plenty of firmwares exploited in order to jailbreak. Lower firmwares, even though they are usually notorious for great stability and success rates, are technically released before newer games. Ex: 5.05 firmware was released back in 2018 while a game like Persona 5 Strikers was released in 2020.
* Sony implemented a check to force the user to update to the latest firmware in order to play newer games (both on digital versions of games and disc games). 
* Clever hackers found a way to disable that check so that no matter what firmware version you have and how old it might be, the game/app could be launched. That kind of patch is called a backport patch.
* Do I need a backport patch? Yes and no. It depends on your firmware. If you are on latest exploitable FW you don't need a backport until a jailbreak for a new firmware will be released (and you decide to stay on your current firmware).
* If you are on a lower firmware you will need a backport patch in order to launch a newer game. Here you can find out what game requries which firmware:
<a href="https://oldnero.github.io/PS4-Games-List/"> PS4 FW Game List </a>

* **NOTE!: There isn't a universal way to backport, some games might work with these methods, while some will not. In any case, there are backports available online by talented devs, so I would recommend you to search them online first (based on your game, version, and region), and only attempt these if you're bored or up for a challenge!**

## Enough talk, let's start...

* Make sure you have your games and updates extracted, everything should be .pkg files.
* Download and extract AutoBackPort Tool:
[AutoBackPortv1.11](/backupfiles/AutoBackPort_1.11.rar)

### For games without updates:
 * Open AutoBackport, set Base Game as the game's .pkg file and set Destination folder to a output folder.
 * Build backported pkg file for the base game. (The result will be a small sized pkg file acting as a fake update)
 * Add the main game pkg and the fake update pkg to the root of a USB drive.
 * Plug the drive to the PS4.
 * Navigate to the PS4 > Settings > GoldHEN > Package Installer and install main game pkg first then the fake update pkg.
 * Done.

### For games with updates:
 * Open AutoBackport, set Base Game as the game's .pkg file, set Update PKG to the .pkg file and set Destination folder to a output folder.
 * Add the main game pkg, update pkg and the fake update pkg to the root of a USB drive.
 * Plug the drive to the PS4.
 * Navigate to the PS4 > Settings > GoldHEN > Package Installer and install main game pkg first, update pkg second then fake update pkg.
 * Done.

## Alternative method if AutoBackPort doesn't work

 * Download, install and save:
    * [downgrade_elf.py script](/backupfiles/downgrade_elf.py)
    * [downgrade_sfo.py script](/backupfiles/downgrade_sfo.py)
    * <a href="https://www.microsoft.com/en-us/p/python-39/9p7qfqmjrfp7?activetab=pivot:overviewtab"> Python </a>
    * <a href="https://github.com/CyB1K/PS4-Fake-PKG-Tools-3.87/archive/refs/heads/main.zip"> FPKG Tools </a>
    * [unfself.exe](/backupfiles/unfself.zip)
    * <a href="https://mh-nexus.de/en/downloads.php?product=HxD20"> HxD Editor </a>
 * In FPKG Tools folder, open orbis-pub-chk.exe. Drag the game pkg to Image List
 * Select Extract files. Enter passcode as all 0's. If the passcode is not 0's, then you need a different pkg.
 * Check Select all files and directories and set a Output directory. Hit Start. Wait and have patience.
 * Drag and drop eboot.bin (extracted from previous step - in Image0 folder) to unfself.exe
 * A new file should appear. Remove eboot.bin and rename the new eboot.bin.decrypted to eboot-old.bin.
 * Open a cmd to the folder you saved the .py scripts.
 * Run following command: downgrade_elf.py --sdk-version 05.050.001 --verbose eboot-old.bin eboot.bin (eboot-old.bin replace with directory of the file). Wait and have patience!
 * Go to Sc0 folder and rename param.sfo to param-old.sfo.
 * Run following command: downgrade_sfo.py --sdk-version 05.050.001 --system-version 05.050.000 --verbose param-old.sfo param.sfo (replace param-old.sfo with directory of the file).
 * Go to Image0 > sce_module folder.
 * Open HxD editor and open libc.prx.
 * Hit Ctrl + F > Hex-values and search for: 18 00 00 00 00 00 00 00 BF F4 13 3C 01 00 00 00 . Replace the next 4 values after highlighted values with: 01 00 05 05
 * Some modules are also linked with other modules. In this case, scroll down until you see a libc.prx decoded text. Last 4 values should have minimum FW too, so replace them with 05 05 00 01. Save file.
 * Repeat the process for the remaining libSceFios2.prx and save the file.
 * Go to Sc0 folder and copy every file to Image0 > sce_sys and replace the files if asked.
 * Open GP4 Generator. In CUSAxxxx Dir put the directory of Image0
 * Select Generate .GP4 and Save .GP4
 * Open orbis-pub-gen.exe.
 * Select .gp4 made and select Build. Set the output folder and select Build again.
 * Done.
 * Install the pkg on your PS4 via Settings > GoldHEN > Package Installer.


## Troubleshooting

 * I installed everything and I get error CE-40740-5. This could be a result of multiple things. Check your PC folder's permissions, available disk space & check and disable AntiVirus if it detected a false postivie. The tool is trusted and completely safe by the PS4 Homebrew community.
