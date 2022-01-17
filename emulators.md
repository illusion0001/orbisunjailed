---
title: "Emulators"
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

## What are emulators and what systems can I play on PS4?

* Emulators are applications that act/behave like a completely different system in order to play games released before / not natively made for PS4.
* On the PS4, there are 2 types of emulators: native (either made by Sony or the company that made/owns the rights to the emulated console) and ports (fan-made emulators).
* Natively the PS4 can emulate PS1, PS2, PSP (but the number of PSP games that work are very low) & Sega Saturn.
* Ports allow the PS4 to emulate MSDOS, NES, every GameBoy, MAME, Atari Lynx, Neo-Geo Pocket, SNES, VirtualBoy, WonderSwan, Nintendo 64, PS1, Sega Genesis/MegaDrive, Nintendo DS, FB Alpha Arcades, Capcom PS1,2 &3, MSX, NEC PC-FX, NEC PC Engine, Sega Saturn, Sega Dreamcast, old PC games, Atari 2600, Atari Jaguar, Vectrex, PSP, various ports, 3DO.

## Enough talk, let's start...

### Native Emulators (PS1, PS2, PSP & Sega Saturn)

#### PS1

* Before attempting, check compatibility list here (if a game is not on the list, feel free to test it):
<a href="https://www.psdevwiki.com/ps4/PS1_Classics_Emulator_Compatibility_List"> PS1 Compatibility List </a>
* Download and extract PSX-FPKG:
   * [PSX-FPKG v.0.2](/backupfiles/PSX-FPKG_v02.7z)
* Download your favourite PS1 rom. Make sure it is in a .bin and .cue file format.
* Launch PS2-FPKG. In the Disc section select the .bin file.
* Rename the tile if it hasn't updated to the game name. Add your own NP Title if it hasn't updated.
* You can select a custom Icon & Background image to make it prettier on the homescreen and when you launch it.
   * Icon resolution must be 512x512
   * Background resolution must be 1920x1080
* Select Create fPKG and wait until it's finished. For multi-disc games you must make new pkg but keeping the same NP Title. When you're done playing a game that requires one disc, save then install and override it with the new pkg.
* Add the created pkg to the root of a USB drive and install it on your PS4 by navigating to Settings > GoldHEN > Package Installer.
* Done.

#### PS2

* Before attempting, check compatibility list here (if a game is not on the list, feel free to test it):
<a href="https://www.psdevwiki.com/ps4/PS2_Classics_Emulator_Compatibility_List"> PS2 Compatibility List </a>
* Download and extract PS2-FPKG:
   * [PS2-FPKG v.0.2](/backupfiles/PS2-FPKG v0.6.7z)
* Download your favourite PS2 rom. Make sure it is either in a .ISO or .bin and .cue file format.
* Launch PS2-FPKG. In the Disc section select the .ISO or .bin file. Also select the other disc .ISO or .bin files in the appropriate section.
* Rename the tile if it hasn't updated to the game name. Add your own NP Title if it hasn't updated.
* You can select a custom Icon & Background image to make it prettier on the homescreen and when you launch it.
   * Icon resolution must be 512x512
   * Background resolution must be 1920x1080
* Select Create fPKG and wait until it's finished.
* Add the created pkg to the root of a USB drive and install it on your PS4 by navigating to Settings > GoldHEN > Package Installer.
* Done.

#### PSP

* Note that even though it is made by Sony, there are only a few games that can be played. Use RetroArch for better compatibility and speed.
* Before attempting, check compatibility list here (if a game is not on the list, feel free to test it):
<a href="https://www.psdevwiki.com/ps4/PSP_Emulator_Compatibility_List"> PSP Compatibility List </a>
* Download and extract PSP HD GUI:
   * <a href="https://github.com/xXxTheDarkprogramerxXx/PS3Tools/releases/tag/PSPHD1.0.0.0"> PSP HD GUI V.1.0 </a>
* Download your favourite PSP rom. Make sure it is either in a .ISO, .CSO or .PBP file format.
* Launch PS2-FPKG. In the Disc section select the .ISO, .CSO or .PBP file.
* Rename the tile if it hasn't updated to the game name. Add your own NP Title if it hasn't updated.
* You can select a custom Icon & Background image to make it prettier on the homescreen and when you launch it.
   * Icon resolution must be 512x512
   * Background resolution must be 1920x1080
* Select Create fPKG and wait until it's finished.
* Add the created pkg to the root of a USB drive and install it on your PS4 by navigating to Settings > GoldHEN > Package Installer.
* Done.

#### SEGA SATURN

* Before attempting, check compatibility list here (if a game is not on the list, feel free to test it):
<a href="https://docs.google.com/spreadsheets/u/0/d/1X4iLL8J5sPMlxr_XbfZ-3f21IF9ni-otn2wwl-4hzsk/htmlview#"> Sega Saturn Compatibility List </a>
* Download and extract SATURN-FPKG:
   * [SATURN-FPKG_v1.1](/backupfiles/SATURN-FPKG_v1.1.7z)
* Download your favourite Saturn rom. Make sure it is either in a .bin and .cue file format.
* Launch PS2-FPKG. In the Disc section select the or .bin file. Also select the other disc .ISO or .bin files in the appropriate section.
* Rename the tile if it hasn't updated to the game name. Add your own NP Title if it hasn't updated.
* You can select a custom Icon & Background image to make it prettier on the homescreen and when you launch it.
   * Icon resolution must be 512x512
   * Background resolution must be 1920x1080
* Select Create fPKG and wait until it's finished. For multi-disc games you must make new pkg but keeping the same NP Title. When you're done playing a game that requires one disc, save then install and override it with the new pkg.
* Add the created pkg to the root of a USB drive and install it on your PS4 by navigating to Settings > GoldHEN > Package Installer.
* Done.


### Emulator Ports

* The majority of the systems, RetroArch is the recommended option.
* Note that RetroArch has been unofficially ported, thus not all cores from PC version might be available.
* Games can be loaded via a USB drive formatted as exFAT. The roms can be placed in a folder.
* Retroarch and it's Core Installer can be downloaded and installed via the Homebrew Store.
* Order of installation: Retroarch Core Installer > Ok to install every core and then RetroArch.
* Done.

## Troubleshooting

 * I built a pkg file with its tool but game either crashes or black screens. In this case the game is not supported.
