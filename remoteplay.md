---
title: "Remote Play"
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

## PC-PS4 Remote Play

### Using patched Remote Play client
 * Note that you will need a PSN account (can be a dummy one and never connected/linked to the PS4).
 * Download and extract the following tools:
    * [Patched Remote Play Client](/backupfiles/PS4 Remote Play 2.6.0.2270.zip)
    * [Remote Play Patcher](/backupfiles/PS4.Remote.Play.Auto-Patcher.zip)

 * Install the patched client. Note: in latest version of Win10 if you get Media Pack error navigate to Settings > Apps > Apps & features > Optional features and remove and install again Windows Media Player.
 * Open Remote Play Patcher and patch it. Note: Windows Defender might block the program. Disable it, file is trusted by PS4 Homebrew community.
 * After jailbreaking your PS4 using GoldHEN navigate to Settings > Remote Play Connection Settings > Enable Remote Play and Remote Play using PSVita/PSTV.
 * Select Add Device and take note of the code.
 * Back to the PC, open Remote Play application, connect to PS4 and sign-in to your dummy PSN account.
 * Select register manually and enter the code.
 * Done.

### Using chiaki (homebrew Remote Play client - also on Mac/Linux and Android's PlayStore)
 * Download and extract following tool:
   * <a href="https://git.sr.ht/~thestr4ng3r/chiaki/refs"> Chiaki Remote Play </a>
 * Open chiaki and select the + icon.
 * For host input your PS4's IP Address. To find out your PS4's IP Address navigate to Settings > Network > View Connection Status.
 * Save and double click the new appear icon.
 * Input your console firmware
 * Input your PSN Account ID (for local accounts and if you used GoldHEN) you can input "fffffffffff=" (That's 11 f's and a = sign). For activated accounts you need the same ID in base 64 format, you can convert it
   * <a href="https://base64.guru/converter/encode/hex"> HEX to Base64 online converter </a>
 * After jailbreaking your PS4 using GoldHEN navigate to Settings > Remote Play Connection Settings > Enable Remote Play and Remote Play using PSVita/PSTV.
 * Select Add Device and input the code in the PIN section of chiaki.
 * Select Register.
 * Done.


## PSVita-PS4 Remote Play

 * PS Vita can connect to hacked PS4 without the need of any additional tweaks (can be regular and hacked Vita).
 * Simply jailbreak your PS4 using GoldHEN.
 * After jailbreaking your PS4 using GoldHEN navigate to Settings > Remote Play Connection Settings > Enable Remote Play and Remote Play using PSVita/PSTV.
 * Select Add Device and input the code in Vita's native Remote Play app (comes with Vita). Do not wait for auto-pair, select skip and input the code.
 * Done.

## Troubleshooting

 * I get choppy audio when I'm using chiaki. Go in chiaki's folder > Audio and remove qtaudio_windows.dll if you're using Windows 10 or qtaudio_wasapi.dll if you're using Windows 7.
 * I get low FPS and/or connection issues using chiaki. Unfortunately this might happen if your connection is not strong enough.
