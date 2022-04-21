---
title: "FPKG Tools"
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

## What are FPKG Tools and what can I do with them?

* FPKG Tools (or Fake PKG Tools), officially known as Publishing Tools, are a collection of utilities used when managing and creating different types of file formats used for PlayStation 4 games and applications.
* This will cover both official (patched from PS4's SDK Publishing Tools) and homebrew tools.

## Tool list

| File Name and extension | Official Name | Tool description | Homebrew Alternative |
| ----------------------- | ------------- | ---------------  |  ------------------  |
| orbis-pub-gen.exe | Package Generator for PlayStation®4 | Package Generator for PlayStation®4 is a software for creating/editing project files (.gp4) and for creating package files (.pkg) for PlayStation®4 using project files | LibOrbisPKG's PKG Editor |
| orbis-pub-sfo.exe | Param File Editor for PlayStation®4 | Param File Editor for PlayStation®4 is a software for creating/verifying the param files (.sfo) required for using applications, patches, additional content, and system software themes for PlayStation®4 | LibOrbisPKG's PKG Editor |
| orbis-pub-trp.exe | Trophy Pack File Utility for PlayStation®4 | Trophy Pack File Utility for PlayStation®4 is a software for creating/verifying the trophy pack files (.trp) required for applications for PlayStation®4 that support the trophy system | None |
| orbis-pub-chk.exe | Image Checker for PlayStation®4 | Image Checker for PlayStation®4 is a software for displaying/verifying image files (package files, ISO image files or compressed ISO image files), etc. and for extracting the files contained in package files | LibOrbisPKG's PKG Editor & PS4PKGVIEWER |
| orbis-pub-cmd.exe | Publishing Tools Command Line Version for PlayStation®4 | Publishing Tools Command Line Version for PlayStation®4 is a software that provides CUI versions of features of the GUI software included in the Publishing Tools, such as Package Generator. Not all the features provided with a GUI are provided in the command line version. On the other hand, there are features that are only provided in the command line version | LibOrbisPKG's PKG Tool |
| vagconv2w.exe and vagconv2.exe | VAG Converter 2 | VAG Converter 2 is a Windows-based tool that converts 16-bit linear PCM waveform data which has been produced using conventional sound tools, into HE-VAG data | None |
| at9tool.exe | ATRAC9 Encoder/decoder | at9tool is an encoding/decoding tool for ATRAC9™ including ATRAC9™ Band Extension (shortened to "ATRAC9™" hereafter except under special conditions) | None |
| gengp4.exe | GP4 Generator for PlayStation®4 | All-in-one utlity to scan a dumped game/application folder structure and generate a .gp4 project file to be used with orbis-pub-gen when creating a PlayStation®4 package | It is already a homebrew application | 

## Download links

* <a href="https://github.com/CyB1K/PS4-Fake-PKG-Tools-3.87"> FPKG Tools - does not include vagconv2 and at9tool </a>
* <a href="https://github.com/OpenOrbis/LibOrbisPkg"> LibObrbisPKG </a>
* <a href="https://sites.google.com/site/theleecherman/ps4pkgviewer"> PS4PKGVIEWER </a>
