---
title: "Linux Installation"
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

## Why should I install Linux?

 * **Note that installing Linux won't override Orbis OS (PS4's main OS) and can only be installed on a external drive!**
 * Installing Linux basically can unlock everything you can do on a normal PC such as desktop emulators, Linux and Steam games & much more.

 * **NOTE!: There isn't a universal way to install Linux, and installing it is on a more technical side, thus this guide is only to be used as a reference. Linux is very troublesome on the PS4 and will varry heavily on what PS4 model, firmware, kernel, distro & many more. Do not attempt if you don't know what you should be doing.**
 
## Enough talk, let's start...

### Requirements

 * A USB 3.0 External drive
 * A USB Keyboard & Mouse (a hub is also recommended)

### USB Drive Setup

 *  Format your drive as FAT32. Huge drives can be formatted via AOEMI Partition Wizard. Make sure it's in MBR Partition Scheme.
 * Download:
     * <a href="https://anonfiles.com/Tdi5B458x6/PS4_Fedora32_MW_Itm.tar_xz"> Fedore32 Linux </a>
     * Hippie68's
[initramfs](/backupfiles/initramfs.cpio.gz)
    * <a href="https://drive.google.com/file/d/1diQPjjYU788-mrw9RfraidsTYv3_zxdD/view"> bzimage </a>
 * Put all the downloaded files on the root of USB drive.
 * Rename PS4_Fedore to psxitarch.tar.xz
 * Jailbreak your PS4 using GoldHEN.
 * Navigate to Settings > System > Disable HDMI Device Link and HDCP.
 * Navigate to Settings > Sound and Screen > Video Output Settings > Set Resolution to 1080p, RGB Range to Full, HDR and Deep Colour Output to Off.
 * Plug the external USB drive to the PS4.
 * Open PS4's Internet Browser and navigate to : https://kar0218.github.io/900CM/index.html. Select Linux 1GB.
 * Wait and have patience. If you see Not Enough Memory errors continue hitting OK until your screen gets dark.
 * Once a wall of text is shown, input: exec install-psxitarch.sh
 * Wait and have patience. After it stopped, input: exec start-psxitarch.sh
 * Wait and have patience. After it stopped, hit Ctrl + Alt + F1 on the keyboard.
 * You are now on the login screem. Input password: linux.
 * Done.
 
 
## Notes and Troubleshooting:

 * After installation, you can switch to a Linux 2GB or Linux 3GB payload.
 * Other distros can be used such as PSXitaArch, Manjaro, Lubuntu, Mint or Gentoo
 * If bzimage doesn't work you can try: <a href="https://gbatemp.net/threads/working-bailkal-linux-kernels-for-ps4pros-on-6-72-and-distros.572063/"> alternatives </a>
