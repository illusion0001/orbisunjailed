---
title: "About & General Knowledge"
site_favicon: "favicon.png"
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

## Why and what exactly is Orbis?

Orbis is PS4's code name used internally by Sony when it was in development. Orbis is also the name of the native operating system of the PlayStation 4, a fork of FreeBSD version 9.0, released on January 12, 2012.


## What does jailbreaking your PS4 mean?

Jailbreaking is, on a basic level, a term used when the console gets exploited to unlock various levels of the firmware that allows the access to many features previously accessible on a DevKit/TestKit (used by game developers and testers) to a consumer.

## What can I do with a jailbroken PS4?

After a successful jailbreak, you can unlock and try the following:

<ul>
	<li>Install and play your game backups/disc games without needing a disc/license/PSN account.</li>
	<li>Access media apps such as YouTube, Netflix without the need of a PSN account.</li>
	<li>Access various homebrew and other fan-made tweaks to your favorite games such as useful applications, fan translations, undubs, emulators, 60FPS patches, etc.</li>
	<li>Make and install custom UI tweaks such as custom dynamic or static themes, removing and hiding useless apps from the homescreen, changing system sounds, etc.</li>
	<li>Access and install a fully featured OS like Linux to completely turn your PS4 into a PC.</li>
</ul>

## What can't I do with a jailbroken PS4?

While the advantages are plenty, you will lose some functionality such as:

 * Online play on **most** games. This is the biggest factor of jailbreaking that many can live without. I used the term most because you can play online on some games by using custom servers, but that is more a bonus than something you should expect.
 * All PSN features such as messaging, online trophy syncing, various PS Plus features such as online save data upload and other features that are dependent on PSN such as Spotify.
 * Depending on the release date of the jailbreak, firmware and games, some newer games will not be available. As soon as new jailbreak will appear, those new games will also appear.
 * **Jailbreaking, regardless of firmware version, is NOT permanent/persistent after reboot or shutdown. Do not compare it to PS3 or Vita, a CFW is almost impossible on PS4, as of today.**


## Useful terms to know

  * Kernel panic = a forced reboot or shutdown caused by the unsuccessful attempt to jailbreak.
  * Webkit exploit = the first part of a full jailbreak, a vulnerability in PS4's Internet Browser (currently every single jailbreak uses this method).
  * Kernel exploit = the second part of a full jailbreak, a vulnerability in PS4's kernel which is the essential center of the operating system (provides basic services for all other parts of the OS).
  * GoldHEN = HEN is a abbreviation of Homebrew Enabler, that allows unlocking the ability to install and play packages (games or apps). GoldHEN is the definitive version of HEN which also adds more features (VR enabler, Remote Package Insalls, Rest Mode support, external HDD supoort, Debug Trophies and many <a href="https://github.com/GoldHEN/GoldHEN#features"> more </a>.
  * Homebrew = the term in PS4's scene, is any piece of application, modification of system that hasn't been directly done by Sony (ex: PS4Xplorer is a fan made file manager in form of a application)
  * Local Account = default type of accounts PS4 can have, meant to be a guest account
  * Activated Account = the other type of accounts PS4 can have, that tricks the system into thinking is a valid PSN account that can unlock some locked features such as save data management (USB only). **Note!: This is not like a actual PSN account, nor you can use it for PSN!**
  * Package (pkg) = the main format PS4 recognizes to pack games, updates, DLC, themes and more (similar to a archive).
  * Payload (in a .bin or .js format) = a file that allows modifying and adding unsigned code to run on the PS4.
  * FTP Transfers = FTP stands for File Transfer Protocol, it is used to remotely send and receive files from and to the PS4 to a PC without the need of USB drives.
  * CFW = Custom FirmWare, a full fan-made firmware, designed for various jailbroken uses. **Note!: PS4 does not have any CFW**.
  * FAKE Packages (fake pkg or FPKG) = Homebrew packages that have not been created or verified by Sony. They are different from retail because they do not need a license or disc to be inserted, but requires the PS4 to jailbroken before attempting to launch them. While the name contains *fake*, they are not malicious, rather a term used to differentiate them from retail packages.
  * RETAIL Packages (retail pkg) = Packages created and verified by Sony that usually come directly from PS Store. These packages cannot be launched if the user does not have a license for the content they wish to launch. Themes however are the only retail packages that can be unlocked.
  * ERROR CODES = error codes are meant for a quick identification of different type of corruptions the PS4 can have. <a href="https://www.psdevwiki.com/ps4/Error_Codes"> A list of error codes and some descriptions can be found here </a>.

## Payloads Explanations

 * **If you are using [Payload Guest](payload-guest.md) or exploit hosts, you might've noticed a few payloads. This will explain what payload does what.**
 * GoldHEN (can be various versions) - the main payload to enable Homebrew (games, apps, themes)
 * Cheat Copy - Copy .json and .shn files from USB to PS4, to be used for GoldHEN Cheat Manager
 * BinLoader - Listens on port 9020 for remote sending payloads (in a .bin format) from PC
 * MiraLoader - Listens on port 9021 for remote sending Mira payload (in a .bin format) from PC
 * Mira - secondary Homebrew Enabler, some payloads need Mira to work correctly
 * WebRTE - payload that enables PS4Trainer
 * PS4Debug - PS4 debugger payload (except kernel mode debugging)
 * Orbis Toolbox - UI payload that enables multiple features such as SOC temperature, FPS, etc.
 * Web Activator - web payload of PS4OfflineActivator, meant to activate local accounts with custom account ID
 * FTP - full access FTP payload
 * App2USB - payload that moves installed games to external HDD/USB drive (does not work if HDD is formatted as external storage)
 * ToDex Enable and Disable - Unlocks some debug features from a DevKit/TestKit such as debug trophies on retail consoles
 * Disable Updates and Enable Updates - payload that creates a PS4UPDATE.pup folder in UPDATE folder to block downloading a update file from Sony servers
 * History Blocker - Disables the automatic loading of last viewed site when launching Internet Browser
 * Enable Browser (outdated / not needed anymore) - payload that permanently enables Internet Browser on firmwares before 5.05
 * Dumper - dumps game/app/kernel modules/modules on a external HDD
 * Linux - Linux loader of various RAM to VRAM modes (1GB to 5GB)
 * DB Backup and DB Restore - Dumps User folder and trophies to a external HDD or USB drive
 * Exit IDU - Disables IDU Mode (Individual Display Unit). This mode is used for display consoles in stores
 * Fan Control - Sets a user determined PS4 fan value to control temperature
 * Rif Renamer (outdated/ not needed anymore) - Converts FAKE license to FREE license to be used on HEN 1.8 (5.05 payload)
 * PermanentUART - payload that enables UART monitoring permanently
 * Disable ASLR - Disables ASLR (Address Space Layout Randomization) to make working with memory easier/repeatable

## Ready to start?

 * Now that you have at least a basic knowledge of what you can do and can't do while jailbroken, <a href="https://florinsdistortedvision.github.io/orbisunjailed/Jailbreak/"> let's continue with the jailbreaking process </a>.
