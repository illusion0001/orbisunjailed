---
title: ".rco Tweaks / UI & Sound Effects Tweaks"
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

## What is a .rco?

* .rco is a proprietary archive format used by PS4 that holds various UI elements such as sound effects.

## Enough talk, let's start...

### Changing PS4 Login Sound

* The login sound can be found in : /preinst/priv/systembgm/ and the file is called bgm_login.at9.
* A .wav file can be easily converted via 
[at9tool](/backupfiles/at9tool.rar)
* To change it, bgm_login.at9 needs to be replaced or renamed to bgm_login.at91 etc, via Full R/W FTP such as GoldHEN.
* Reboot

### Changing PS4 Background Music
 
 * The background music can be found in : /system_ex/app/NPXS20001/systembgm/ and the file is called bgm_main.at9.
* A .wav file can be easily converted via 
[at9tool](/backupfiles/at9tool.rar)
* To change it, bgm_main.at9 needs to be replaced or renamed to bgm_main.at91 etc, via Full R/W FTP such as GoldHEN.
* Reboot

### Changing System Sounds

 * All the files can be found in: /system_ex/vsh_asset/ and the file is called Sce.PlayStation.PUI.rco (previously named Sce.PlayStation.HighLevel.UI2.rco, not sure at what point a new firmware changed that).
 * The .rco can be easily extracted via <a href="https://bitbucket.org/SilicaAndPina/cxml-decompiler/src/master/"> cxml-decompiler v8 </a>. Must be the latest v8 version!
 * The files converted will be in a .vag format. Most of them are 0:01 or 0:02 seconds in length, in .vag 4-bit ADPRCM 438kps at 48kHz stereo files.
 * A .wav file can be easily converted via
[at9tool](/backupfiles/at9tool.rar)
 * Note!: Analyze your audio and check if you have any silence and remove it accordingly to make sure your sound effects will play and end right!
 * The system sounds are named accordingly now (starting with the latest version of cxml-decompiler) and can be previewed in the extracted directory "Sce.PlayStation.PUI/files/converted/VAGtoWav". Note!: These files are only for listening mainly, do not bother to replace these with your .wav as nothing will happen!
 * After you converted your files to .vag, you must replace your desired sound in "Sce.PlayStation.PUI/files/original". Example: snd_cursor1.vag - default homescreen cursor sound
 * After you replacing your files, via a cmd terminal run the following command: "CXMLDecompiler.exe Sce.PlayStation.PUI\Sce.PlayStation.PUI.xml -c" to re-compile the file back. Note that it will make the file with the name "-c" so you must rename it back to Sce.PlayStation.PUI.rco.
 * FTP back to your PS4 to the same directory (/system_ex/vsh_asset/) and replace the file. Note!: You must have full R/W permissions to replace. Either use OrbisFTP or for GoldHen v2 users via your FTP client run the following command (ex: if using FileZilla - Server - Enter custom command) - "MTRW" in all caps!
 * Reboot your PS4.
 * Done.

## Final notes!:

 * All changes are persistent after reboot.
 * If you have a custom theme, all those sounds will be replaced with the theme sounds. To test them, go back to a default PS4 theme like Flow.
 * If you want to go back to the default files I provided the original Sce.PlayStation.PUI.rco file here: <a href="https://anonfiles.com/t5SdhdBcx0/Sce.PlayStation.PUI_rco"> Sce.PlayStation.PUI.rco </a>. Replace it the same way you did before (with Full R/W permissions!)
