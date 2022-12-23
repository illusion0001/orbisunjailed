---
title: "entitlement.db - Reinstall your removed PSN games"
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

## What are entitlements and what can I do with them?

* entitlements.db is the file that holds a database of every single content (game, update, DLC, themes) installed from PS Store from when the PS4 was on latest firmware at some point.
* By viewing the file, you can find direct package links to the content from PS Store, thus allowing to reinstall them again.
* **Do note that your licenses must be intact (can be invalidated anytime if your PS4 has connected to internet without DNS). If you still install them without a license, your content will forever have a padlock next to it and CAN'T be unlocked** *(themes are the only exception however)*.

## Enough talk, let's start...

* Jailbreak your PS4 with GoldHEN.
* Navigate to Settings > GoldHEN > Enable FTP. Take note of the IP Address.
* Open FileZilla and input PS4's IP Address on host and 2121 on port.
* FileZilla > Server > Enter custom command > MTRW (must be all caps).
* Navigate to /system_data/priv/license and copy entitlement.db to Desktop.
* Open HxD, search for .json. For newer content, it may be stored in a .xml file.
* On your PC's browser, navigate to https://store.playstation.com/ and make sure you're logged in.
* Copy the .json and/or the .xml link you found in HxD, and paste it to the web browser.
* You now have access to your entitlements database.
* Example for what you should find:

`{"originalFileSize":13368819712,"packageDigest":"3DB8AEC764D7FAF765A07A1B66E30D2ECB146FA94FA1C4C9DE437FAA3ECC2703","numberOfSplitFiles":4,"pieces":[{"url":"http://gs2.ww.prod.dl.playstation.net/gs2/appkgo/prod/CUSA14836_00/1/f_d920437d66cd1b322f80229f61ee586364933e62ad996fb13281a967190a9ba1/f/UP2611-CUSA14836_00-CATHERINEFBUS009_0.pkg","fileOffset":0,"fileSize":4294967296,"hashValue":"4cd746a68003045a7f54e77bcdf58eef5f842fc9"},{"url":"http://gs2.ww.prod.dl.playstation.net/gs2/appkgo/prod/CUSA14836_00/1/f_d920437d66cd1b322f80229f61ee586364933e62ad996fb13281a967190a9ba1/f/UP2611-CUSA14836_00-CATHERINEFBUS009_1.pkg","fileOffset":4294967296,"fileSize":4294967296,"hashValue":"5efcc9500ade8438ca14b66760dd6be6ac3c8faf"},{"url":"http://gs2.ww.prod.dl.playstation.net/gs2/appkgo/prod/CUSA14836_00/1/f_d920437d66cd1b322f80229f61ee586364933e62ad996fb13281a967190a9ba1/f/UP2611-CUSA14836_00-CATHERINEFBUS009_2.pkg","fileOffset":8589934592,"fileSize":4294967296,"hashValue":"68dfe705e67d60bfc05b9d86acfd65bcbbdff737"},{"url":"http://gs2.ww.prod.dl.playstation.net/gs2/appkgo/prod/CUSA14836_00/1/f_d920437d66cd1b322f80229f61ee586364933e62ad996fb13281a967190a9ba1/f/UP2611-CUSA14836_00-CATHERINEFBUS009_3.pkg","fileOffset":12884901888,"fileSize":483917824,"hashValue":"b9d5e625f581b38b6f60e8c67d0562bb080a52b6"}]}`

* Simply take all the urls to a new page and download them all.
* You can then put them all on a USB drive and install them via Debug Settings.
* Done.

### More questions and answers

* **All my games, DLC and themes have padlocks on them!**
    - If your content has a padlock, it means your licenses are no longer valid (have been invalidated by Sony's server when you connected your PS4 to internet on older firmware). 
    - Unfortunately you cannot do anything to fix it, however **retail themes** can be unlocked via a unlocker. [See here for a guide](retail-theme-unlock.md).
* **My entitlement.db file is empty!**
    - If your database is empty it's probably because you either never installed anything from PS Store on your PS4 or you did a clean install of your current firmware, removing everything in the process.
    - Nothing you can do to fix it, unfortunately.
* **Can I take the entitlements.db from another PS4 to my jailbroken one?**
    - No, even if you do it you cannot transfer your licenses so your content will forever have a padlock. Licenses are both console specific and account specific.
