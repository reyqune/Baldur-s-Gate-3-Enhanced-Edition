
![](https://raw.githubusercontent.com/reyqune/Baldur-s-Gate-3-Enhanced-Edition/main/images/Banner.png)

<p align="center">
  [ <a href="https://www.nexusmods.com/skyrimspecialedition/mods/118893">Nexus</a> |
  Installation |
  <a href="https://github.com/Oghma-Infinium/Apostasy/blob/main/GAMEPLAY.md">Gameplay Guide</a> |
  <a href="https://github.com/Oghma-Infinium/Apostasy/blob/main/CHANGELOG.md">Changelog</a> |
  <a href="https://loadorderlibrary.com/lists/Apostasy">Modlist</a> |
  <a href="https://github.com/Oghma-Infinium/Apostasy/blob/main/Documentation/FAQ.md">FAQ</a> |
  <a href="https://github.com/Oghma-Infinium/Apostasy/blob/main/Documentation/CONFIG.md">Configuration</a> |
  <a href="https://github.com/Oghma-Infinium/Apostasy/blob/main/Documentation/ADDONS.md">ADDONS</a> |
  <a href="https://ko-fi.com/reyqune">Ko-fi</a> ]
</p>

---

**Modlist Support: [reyqune's discord server](https://discord.gg/QjBtu2JA)**

>[!IMPORTANT]
>Apostasy requires the four free AE mods (Fishing, Rare Curios, Survival Mode, and Saints and Seducers) included in the Skyrim Anniversary Edition update from November 2021.

>[!WARNING]
>You must update Skyrim to the latest version (1.6.1170) on Steam to install this list.

# Contents

- [Contents](#contents)
  - [Introduction](#introduction)
    - [System Requirements](#system-requirements)
    - [Video Guide](#video-guide)
  - [Installation](#installation)
    - [Pre-Installation](#pre-installation)
      - [Installing Microsoft Visual C++ and .NET](#installing-microsoft-visual-c-and-net)
      - [Pagefile and Crash Prevention](#pagefile-and-crash-prevention)
      - [Setting Shader Cache Size (NVIDIA Users Only)](#setting-shader-cache-size-nvidia-users-only)
      - [Steam Setup](#steam-setup)
      - [Changing the Game Language](#changing-the-game-language)
      - [Installing Rare Curios Files](#installing-rare-curios-files)
    - [Wabbajack Installation](#wabbajack-installation)
      - [Installing Wabbajack](#installing-wabbajack)
      - [Downloading and Installing Apostasy](#downloading-and-installing-apostasy)
    - [Problems with installation](#problems-with-installation)
      - [Problematic Files](#problematic-files)
  - [Post-Installation and Optional Setup](#post-installation-and-optional-setup)
    - [Game Folder](#game-folder)
    - [Antivirus Exceptions](#antivirus-exceptions)
    - [Post-Installation Issues and Troubleshooting](#post-installation-issues-and-troubleshooting)
    - [Keyboard Keybinds](#keyboard-keybinds)
    - [Gamepad Keybinds](#gamepad-keybinds)
  - [Playing the List](#playing-the-list)
    - [Starting the Game](#starting-the-game)
  - [Updating the modlist](#updating-the-modlist)
  - [Removing the Modlist](#removing-the-modlist)
  - [Issues](#issues)
  - [Credits and Thanks](#credits-and-thanks)

## Introduction

Apostasy is a Wabbajack modlist for Skyrim SE that offers a modern, action-oriented combat system, custom tailored gameplay, and a consistent, high-fidelity graphics overhaul. Apostasy aims to deliver a cohesive and refined experience, enhancing both visuals and mechanics.

A full list of the mods used in this modlist can be viewed [here](https://loadorderlibrary.com/lists/Apostasy).

You can find a summary of all relevant gameplay changes on the [Gameplay Guide](https://github.com/Oghma-Infinium/Apostasy/blob/main/GAMEPLAY.md) as well.

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

### System Requirements

The listed specs are the best idea of a baseline that I can provide at the current moment, based on feedback I have gotten from testers and my own experiences. In the future this will be updated depending on feedback received. Your PC may run the list better or worse due a variety of reasons, **I will not provide troubleshooting or support for hardware related issues.**

>[!WARNING]
>
>- An SSD is **required** to the play the modlist.
>- Only Windows 10 or 11 operating systems are supported. Windows LTSC, special variants, lightened editions or any other modified variant **WILL NOT WORK.** Linux installations also **WILL NOT WORK**.

![](https://raw.githubusercontent.com/Oghma-Infinium/Apostasy/main/images/perfTarget.PNG)

<Details>
<summary>Clarification on PC Requirements</summary>

For complete clarity, my specs while building the list were a 5800X, 2080, and 32GB of RAM. This PC ran the list @ 50-60FPS on 1440p (16:9).  
My current specs are a 7800X3D, 3080, and 32GB of RAM with some BIOS tweaks (ReBar and PBO mostly). This PC runs the list @ stable (locked) 61FPS on 1440p (16:9).

</Details>

Downloads Size: ~160 GB  
Install Size: ~190 GB  
Temporary Files: ~40 GB (on OS drive)  
**TOTAL:** ~350 GB  

> The **Install Size** listed on the Wabbajack Gallery is **wrong** and does not properly account of the size saved by compressing files during the installation.

<Details>
<summary>Info on Temporary Files</summary>

Wabbajack typically requires around 30-40 GB of space on your main OS drive for temporary and working files during the installation, this space is not counted towards the total install space of the list for sake of this guide, however Wabbajack roughly accounts for it in the UI.

</Details>

<Details>
<summary>BSA Warning</summary>

Apostasy heavily employs [BSA](https://en.uesp.net/wiki/Skyrim_Mod:Archive_File_Format)s in order to keep the list's size down and improve performance. However, this means that the installation process may take longer than some other lists and you may run into issues with Wabbajack crashing if you allocate too many system resources to it. It also can potentially inflate the amount of temporary file space required by Wabbajack but this still needs to be tested and confirmed.

If you are struggling with issues of Wabbajack crashing during the installation process, please read the [Problems with Installation](#problems-with-installation) section of this ReadMe.

</Details>

### Video Guide

If you would prefer to follow along with a video guide, you can watch the Installation Guide by clicking the image below.

[![](https://raw.githubusercontent.com/Oghma-Infinium/Apostasy/main/images/InstallThumbnail.png)](https://youtu.be/6IJlT_H7pvk?si=OldwShLFkc1-W9Xq)

## Installation

Installing Apostasy is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#updating-the-modlist).

### Pre-Installation

These steps are only required for installing the modlist for the first time. Additionally, many of these steps may be covered in other modlist installs, for new users I suggest reading through here regardless.

#### Installing Microsoft Visual C++ and .NET

 1. Install [Visual C++ x64](https://aka.ms/vs/17/release/vc_redist.x64.exe).
 2. Install [.NET Runtime 8.X.X Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/8.0).
 3. Install [.NET 6.0 Runtime Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.30-windows-x64-installer).

>[!WARNING]
>If you already have Visual C++ installed, please make sure you install it again and use the `Repair` option to get the latest version of the redistributables. **Do NOT skip this step or MO2 and the game may fail to launch.**

#### Pagefile and Crash Prevention

>[!WARNING]
>Larger Skyrim modlists require a significant amount of memory, running out of memory **will** result in crashes and other potential issues. Due to Apostasy's size and number of files, this step is **NOT** optional. I do not care how much RAM or VRAM you have, please do this step.

**To set up a Pagefile:**

 1. Press `Win Key + R`
 2. Type `sysdm.cpl ,3` and hit `ENTER`
 3. Navigate to **Performance** and click the box `Settings...`
 4. Click the **Advanced** tab at the top
 5. Under **Virtual Memory** click the box `Change...`
 6. Uncheck `Automatically Manage` if it is checked
 7. Select your disk drive, ideally your fastest solid state drive
 8. Click `Custom Size:`
 9. In the box next to **Initial Size (MB)**, type `40960`
 10. In the box next to **Maximum Size (MB)**, type `40960`
 11. Click `Set`.
 12. Click `OK`.
 13. Click `Apply`.
 14. Click `OK`.
 15. **Restart your PC**.

>[!TIP]
> Your pagefile does not need to be on the same drive as your Wabbajack install or Steam install.

<Details>
<summary>Bonus Reading: Why do we need a Pagefile?</summary>

Skyrim is a very old game (originally released in 2011) that is built on the [Creation Engine](https://en.wikipedia.org/wiki/Creation_Engine), a engine based off of the [Gamebryo](https://en.wikipedia.org/wiki/Gamebryo) engine that was originally used for Morrowind (released in 2002).

Through lots of experience and trial-and-error, we have discovered that increasing the window's pagefile can fix certain types of Skyrim crashes, the two most common examples being `Unhandled native exception occurred at 0x7FF6ADC8DDDA` and `Unhandled native exception occurred at 0x0`.

But why is this? Skyrim appears to use system memory in very unexpected ways, for example it will frequently dip into the pagefile memory despite there being available RAM. Skyrim heavily favors high speed, low latency RAM (the best you can get as of writing this is 6000MHz and CL30 for DDR5).

</Details>

#### Setting Shader Cache Size (NVIDIA Users Only)

>[!IMPORTANT]
>For NVIDIA users, it is recommended to boost the size of the shader cache. These settings have been shown to improve stability, while it may not be entirely necessary, it is still recommended.

**To do this:**

- Right-click on your desktop and select `NVIDIA Control Panel`
- Navigate and click `Manage 3D Settings`
- Scroll down the **Global Settings** tab until you see **Shader Cache Size**
- Double-click `Driver Default` to the right of **Shader Cache Size** and select `10 GB`
- Click `Apply` in the bottom right hand corner
- Exit out of the application
![](https://raw.githubusercontent.com/iAmMe27/Tahrovin/main/img/ShaderCache.png)

#### Steam Setup

>[!WARNING]
>If you have your Steam Library in Program Files, read [this article](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) by LostDragonist. Locations such as Desktop, Documents, Downloads, OneDrive, etc. *will* cause issues with installing and playing the list.

 1. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
 2. Right click on Skyrim SE and click on properties, untick the `Enable Steam Overlay while in-game.`
 3. Please ensure you follow the steps outlined in the [Installing Rare Curios Files](#installing-rare-curios-files) section. **DO NOT SKIP THIS STEP OR YOUR INSTALL WILL FAIL.**

#### Changing the Game Language

>[!WARNING]
>**The English Steam version of Skyrim SE is the only supported version.**

I understand that this may be frustrating for non-English speaking users or users with the GOG/Bethesda.net versions, but due to the core file differences between the different versions, I am only able to support one game version.

To change your Skyrim SE's language:

 1. Right click on Skyrim SE in Steam
 2. Click `Properties`
 3. Click `Language`
 4. Set the Language to `English`

#### Installing Rare Curios Files
>
>[!WARNING]
> ***Do NOT skip this step or your install may fail!***

From the 1.6.1130 update and onwards, Steam now ships Skyrim with its own version of the free CC files. However these files do not have the same hashes as the files that are downloaded from the in-game Creation Club menu for AE users. In order to work around this issue and make the list as accessible as possible, the list is compiled using the file hashes from the in-game CC downloads.

To download Bethesda's version of Rare Curios:

- Navigate to your Skyrim SE's Steam Data folder
  - i.e. `D:\SteamLibrary\steamapps\common\Skyrim Special Edition\data`
- Delete *both* Rare Curios files:
  - `ccbgssse037-curios.bsa`
  - `ccbgssse037-curios.esl`
- Launch Skyrim SE from Steam and select **Creations** at the main menu
- Select **Search** at the bottom and search for `Rare Curios`
- Select the card titled `Rare Curios` and press **Download**
- Once it is done, accept Bethesda's load order message and exit the game

![](https://cdn.discordapp.com/attachments/1008055818782003421/1263168806054920283/Rare_Curios.png?ex=669a929f&is=6699411f&hm=9441dc9f4f9e95a4ac3e890de860d406884be4b88dc8e8d8309a2ff3f93830b9&)

>[!IMPORTANT]
>
>- **DO NOT** Alt+Tab during this process or it will fail to properly download these files
>- **DO NOT** verify your game files after doing the steps above as it will revert the "correct" file hashes for the Rare Curios files

### Wabbajack Installation

#### Installing Wabbajack

Once you have completed the pre-installation section, follow these steps to install Wabbajack:

1. Create an empty folder named `Wabbajack` on the root of your drive, such as `C:\Wabbajack` for example.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), in your Skyrim's Steam folder, or in any folders related to the modlist itself (the downloads or install folder).**
    > - The `Wabbajack` folder does not need to be on an SSD, but it makes installing faster. You can set this location to be on an HDD for the sake of saving space.

2. Download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases/latest/download/Wabbajack.exe) and place the `Wabbajack.exe` file inside the Wabbajack folder you created in Step 1.

3. Double-click the `Wabbajack.exe` file that is now inside your Wabbajack folder to set up the program.

>[!IMPORTANT]
>The list requires Wabbajack version **3.6.1.0 or later**. Installing the modlist on older versions of Wabbajack will prevent the installation from being completed.

#### Downloading and Installing Apostasy

>[!CAUTION]
>**A legal copy of Skyrim Special Edition is required.** Pirated copies of the game will cause the installation to fail and even if you manage to somehow get around Wabbajack's built-in piracy prevention measures, SKSE does not work with the cracked exes.  

Downloading and installing Apostasy can take a while depending on your internet connection, PC specs, and if you have Nexus Premium. Without Premium, you will need to manually click the **Slow Download** button for each mod.

To install Apostasy, complete the following steps.

 1. Open Wabbajack and click `Browse Modlists`
 2. Tick on the `Show Unofficial Lists` box and pick the **Skyrim Special Edition** option from the game filter drop-down box (or use the search bar to find the modlist)
 3. Press the download arrow on the Apostasy UI card and wait for it to download
 4. Set the `Modlist Installation Location` to a folder such as `C:\Apostasy`.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), or in your Skyrim's Steam folder**
    > - The `Resource Download Location` does not need to be on an SSD, but it makes installing faster. You can set this location to an HDD for the sake of saving space.
 5. Download the files from the [Problematic Files](#problematic-files) section and place them in your designated `Resource Download Location` folder.
 6. Press the play arrow to begin.
 7. Turn on your favorite show or a nice long video essay as Wabbajack does its thing. Alternatively read through this readme again.
 8. If the installation is successful, then rejoice and move onto [post installation](#post-installation-and-optional-setup). If the installation is unsuccessful, follow the tips below or the [discord server](https://discord.gg/4WwqfK5yHg) for support.

### Problems with installation

It is possible that you may encounter an error with Wabbajack when installing. Some common issues are listed below.

<Details>
<summary>I'm having trouble downloading Non-Nexus files or specific files!</summary>

Big files can fail to download due to connection issues or website issues. You can either run Wabbajack again or download the missing file manually. If you decide to manually download the file, make sure to place the file(s) inside the folder you set as the `Resource Download Location`.

This issue can also occur with files sources from Google Drive, MEGA, Patreon, and other sites. If you are failing on a non-nexus file, then read the [Problematic Files](#problematic-files) section.

</Details>

<Details>
<summary>Wabbajack couldn't find my game folder!</summary>

Either buy the game or re-read the [Pre-Installation](#pre-installation) section.  

</Details>  

<Details>
<summary>My antivirus reports a virus with the program or modlist!</summary>

Windows 10/11 may automatically quarantine a key file which is needed for Mod Organizer. You can fix this by [adding an exclusion for Mod Organizer in windows defender](#antivirus-exceptions).  

</Details>

<Details>
<summary>Unable to download 'Data_ccbgssse037-curios': </summary>

Please make sure you are following the steps outlined in the [Installing Rare Curios Files](#installing-rare-curios-files) section

</Details>  

<Details>
<summary>Unable to download Skyrim_Default.ini:</summary>

This error means you failed to follow this Readme. Go back and follow the steps outlines in the [Changing the Game Language](#changing-the-game-language) section

</Details>  

<Details>
<summary>Sanity check error extracting file:</summary>

Wabbajack will sometimes have issues extracting files if they use special characters. If you encounter this issue in a Wabbajack log, please try the steps down below:

 1. Press `Win Key + R`.
 2. Type `intl.cpl` and hit `ENTER`.
 3. Navigate to *Administrative* and click `Change system locale...`.
 4. Change the *Current system locale:* to `English (United Kingdom)`.
 5. **Uncheck** `Beta: Use Unicode UTF-8 for worldwide language support`
 6. Click `OK`
 7. **Restart your PC** and rerun the Wabbajack installer.

</Details>  

<Details>
<summary>Wabbajack is crashing during the installation!</summary>

If you find yourself struggling to run Wabbajack without it crashing, freezing up, or blue-screening your PC, please try lowering Wabbajack's resource usage with these steps:

 1. Open Wabbajack.
 2. Click the gear icon in the top-right corner of the Wabbajack window.
 3. Click the `Edit Resource Usage Settings and Close Wabbajack` button.
 4. Lower the `MaxTasks` number for each category to half of what it is currently set to.
 5. Press `Ctrl+S` on your keyboard to save the file.
 6. Open Wabbajack and continue the installation process.

>[!TIP]
> It is suggested to have a program installed on your PC that can open `.json` files, like [Notepad++](https://notepad-plus-plus.org/) or [Visual Studio Code](https://code.visualstudio.com/)

</Details>  

#### Problematic Files

Wabbajack frequently has trouble downloading mods hosted on sites other than Nexus. These files are listed below for your convenience. You will need to manually download these files and place them in the `Resource Download Location` that is made in the [Downloading and Installing Apostasy](#downloading-and-installing-apostasy) section.

Google Drive Files:

- [High Poly Head v1.4 (SE)](https://drive.google.com/uc?id=15_0njBUjHKidNnJPmLXEygzGVWsA3Zbq&export=download)
- [Dint's BDOR Hairs](https://drive.usercontent.google.com/download?id=1tpY3bDs-LR6rptf8oPUfraKs1CkxJJB3&export=download&authuser=0)
- [Dint's HairPack 02](https://drive.usercontent.google.com/download?id=1Ts0sQz3hDxhCeS_LUnXJQFuws_qbw9YQ&authuser=0)
- [Dint's Face Part mod](https://drive.usercontent.google.com/u/0/uc?id=1RQl8ki73fgLnzBZn6EWjneuW4Dk8TUO_&export=download)
- [Olivier Kenjutsu Battleaxe and Warhammer](https://drive.google.com/file/d/1rX4INfO3ieWp25gPh0NiLPl1ktLoegZ9)

MEGA Files:

- [High Poly Head - EFA - Male Eyebrow fix](https://mega.nz/file/WZt0BDCL#JNUTn_5P2sEPuHm3znSdrrqN28tPnxvmVzeFOw67FAU)

Patreon Files: (These are free to download)

- [ESkyrim MCO Installer](https://www.patreon.com/file?h=68233071&i=11449877)
- [HDT-SMP Sona Armor - Female](https://www.patreon.com/file?h=68902488&i=12781379)
- [HDT-SMP Sona Armor - Male](https://www.patreon.com/file?h=68902488&i=13158956)
- [Highlander Armor - Female](https://www.patreon.com/file?h=79874952&i=13365775)
- [Highlander Armor - Male](https://www.patreon.com/file?h=79874952&i=13365782)
- [HDT-SMP Melony Armor](https://www.patreon.com/file?h=67711235&i=10980531)

## Post-Installation and Optional Setup

### Game Folder

Apostasy uses a Wabbajack feature called Stock Game to keep your Skyrim installation clean. All the files that you need to run the list are in a folder called `Stock Game`. You don’t need to copy anything at all.

### Antivirus Exceptions

>[!WARNING]
>Antivirus programs are notorious for false flagging [MO2's Virtual File System](https://stepmodifications.org/wiki/Guide:Mod_Organizer/Advanced), which can and will cause crashes and other problems. Antivirus programs like BitDefender, Norton, and Webroot are especially aggressive, and you will very likely need to fully remove them from your PC in order to actually launch the game through MO2. It is 2024, Windows Defender and being smart online is more than adequate to protect yourself from malicious software.

If you use Windows Defender, it is advised that you set up an exception for the modlist.

<Details>
<summary>Setting up Windows Defender Exceptions:</summary>

 1. Press the Windows Key.
 2. Type "Windows Defender" in the search bar and select "Windows Security".
 3. Click on "Virus & threat protection" in the left pane.
 4. Click the "Manage settings" option under "Virus & threat protection settings".
 5. Scroll down to "Exclusions" and click "Add or remove exclusions".
 6. Windows Defender will prompt you with a run as administrator screen, just hit yes.
 7. Click the "Add an exclusion" button at the top and choose "Folder".
 8. Navigate to your Install folder for the list and click "Select Folder".
 9. **(OPTIONAL)** You can repeat these steps for the other executables:
    - ModOrganizer.exe (`[Path to Modlist]\ModOrganizer.exe`)
    - Nemesis Unlimited Behavior Engine.exe (`[Path to Modlist]\mods\Project New Reign - Nemesis Unlimited Behavior Engine\Nemesis_Engine\Nemesis Unlimited Behavior Engine.exe`)
    - Synthesis.exe (`[Path to Modlist]\tools\Synthesis\Synthesis.exe`)

</Details>  

### Post-Installation Issues and Troubleshooting

<Details>
<summary>Game is zoomed into the top left corner!</summary>

Windows Scaling can prevent games from displaying correctly, and will often result in the game appearing "zoomed in". To fix this, find the `SkyrimSE.exe` located in your `[Path to Modlist]\Stock Game` and follow the steps in the images below:

![](https://raw.githubusercontent.com/Oghma-Infinium/Apostasy/main/images/skyrim-scaling.png)

</Details>

<Details>
<summary>Form 43 Error in MO2. / A DLL plugin has failed to load correctly.</summary>

Your installation did not complete. Rerun Wabbajack and make sure to tick the **Overwrite Installation** box. If the error persists after a reinstall, then delete the `[Path to Modlist]\mods` folder, and rerun Wabbajack again.

</Details>  

<Details>
<summary>Crashing on Startup</summary>

Report it in the `#apostasy-support` channel of the [discord](https://discord.gg/4WwqfK5yHg). There are several reasons why this might happen, and 99.9% of them are a corrupt installation.

</Details>  

<Details>
<summary>Crashes during Gameplay</summary>

Skyrim is a notoriously buggy game and cramming thousands of mods into it is not gauranteed to always produce the most stable experience possible. Especially in heavier lists where you may be pushing the limitations of your hardware as a result of Skyrim's old and unoptimized rendering pipeline.

If you find yourself crashing, then please share your crashlogs in the appropriate #support channel on the [discord server](https://discord.gg/4WwqfK5yHg).

In order to get the best possible response please ensure that:

 1. Your crash is reproducible.
 2. You include all relevant crashlogs (if you do not know where to find them then use the `!crashlog` command in chat).
 3. Provide details about the crash (what you were doing, where it took place, if there was an associated quest, etc). Details are necessary in order to quickly diagnose crashes.

</Details>  

<Details>
<summary>Crashes When Loading Saves</summary>

This issue is caused by Large Reference Workarounds done by [DynDOLOD NG](https://www.nexusmods.com/skyrimspecialedition/mods/97720) Due to importance of the mod, it cannot be removed from the modlist.

Follow the steps below for a temporary experimental fix to prevent these crashes:
  1. Navigate to `[Your Apostasy Install Location}\profiles\Apostasy\SkyrimPrefs.ini`  
  2. Change `uLargeRefLODGridSize =9` to `uLargeRefLODGridSize =5`  
  3. Press `Ctrl+S` on your keyboard to save your changes

This will reduce the quality of certain large objects at far away distances, however the difference is **very minor** and you will be unlikely to even notice it. Changing these settings may even improve performance.

</Details>

### Keyboard Keybinds

![](https://raw.githubusercontent.com/Oghma-Infinium/Apostasy/main/images/Keybinds.png)

### Gamepad Keybinds

>[!WARNING]
>Gamepads may need additional setup in order to work as intended. Please refer to the [Configuration](https://github.com/Oghma-Infinium/Apostasy/blob/main/Documentation/CONFIG.md#gamepad-support) page.

![](https://raw.githubusercontent.com/Oghma-Infinium/Apostasy/main/images/controlmap.png)

>[!TIP]
>You can review default keybinds in game by pressing `F11`!

## Playing the List

>[!WARNING]
>Before starting the list, read over the [Configuration](https://github.com/Oghma-Infinium/Apostasy/blob/main/Documentation/CONFIG.md), [FAQ](https://github.com/Oghma-Infinium/Apostasy/blob/main/Documentation/FAQ.md), and [Gameplay](https://github.com/Oghma-Infinium/Apostasy/blob/main/GAMEPLAY.md) pages.

### Starting the Game

 1. Head over to your modlist installation folder (e.g. `C:\Apostasy`), locate an executable named `ModOrganizer.exe`, and launch it. Your first launch of Mod Organizer 2 may take several minutes due to GitHub repository downloads, so please be patient.
 2. Set up your CPU Affinity by following the instructions below. Please do not skip this step
    <Details>
    <summary>Setting CPU Affinity</summary>
    
    This section is also covered in the [Configuration Guide](https://github.com/Oghma-Infinium/apostasy/blob/main/Documentation/CONFIG.md#performance-optimizations).

    [Skyrim Priority](https://www.nexusmods.com/skyrimspecialedition/mods/50129) is a mod that can greatly improve performance, improving FPS and preventing stutters by optimizing Skyrim's CPU Priority and Core Affinity. [CPU Affinity](https://www.nexusmods.com/skyrimspecialedition/mods/94636) is a Mod Organizer 2 plugin that automates the manual setup of [Skyrim Priority](https://www.nexusmods.com/skyrimspecialedition/mods/50129). However, when improperly configured it can lead to worse performance than if it had not been present.

    Due to Wabbajack limitations, the mod must be manually adjusted on the end-user's system. In order to do this follow the instructions below:

    1. Click the `Puzzle Piece` button at the top of MO2 and select `Set CPU Affinity` and press `OK` on the pop-up box.
  
        ![](https://raw.githubusercontent.com/Oghma-Infinium/Vagabond/main/images/cpu%20affinity%20example.png)  

    2. That's it, it's really that simple. **Please, please, please** do this before launching the game and whenever you update the modlist.

    </Details>

 3. Launch the "Play" Executable in MO2. The game may take several minutes to load on your first launch. Please be patient and **DO NOT** click the `Unlock` button on the MO2 prompt.
    a. **I REPEAT, DO NOT CLICK THE UNLOCK BUTTON! YOU WILL BREAK YOUR GAME!**
 4. Select the **New Game** button.
 5. Create your lovely character.
 6. **(OPTIONAL)** Refer to the different MCM options listed on the [Configuration](https://github.com/Oghma-Infinium/Apostasy/blob/main/Documentation/CONFIG.md#in-game-mcm-options) to adjust any MCM settings you'd like.
 7. Pick your class and talk to the little Dragon sitting on a lantern. If no specified start is chosen, then you will have the default start in the Helgen Inn.
 8. Simply open the door next to him and step into the black void gazing at you :)

## Updating the modlist

Versioning for the list will adhere to the following format: `MAJOR.MINOR.PATCH`.

- `MAJOR`: Any release with a number change here will be considered a major update as at least 1 area of the list was massively overhauled. These updates with **NEVER** be save safe.
- `MINOR`: Any release with a number change here will be considered a minor update, these updates will usually not be save safe, unless otherwise specified.
- `PATCH`: Any release with a number change here will be considered a patch, these updates should be save safe and will be used primarily for bugfixes.
- In some rare cases you may see a fourth slot be used, which I will refer to as `HOTFIX`. These list "updates" will be used if the list needs to be recompiled for any reason. There will be no changes in these "updates" as they are purely for maintenance.

Updating is like installing the list. Simply make sure your paths are the same and tick the `overwrite installation` button. Please keep in mind any mods you have added will be deleted when updating. To make sure that Wabbajack does not delete your added mods upon updating, prefix your mods with `[NoDelete]`.

>[!IMPORTANT]
>Saves can be continued across **Save-Safe** updates. Updates will be indicated whether or not they are **Save-Safe** on the [Changelog](https://github.com/Oghma-Infinium/Apostasy/blob/main/CHANGELOG.md). It is suggested that you backup your saves before updating if you plan on continuing them.

>[!TIP]
>RaceMenu presets can be placed in the `[NoDelete] RaceMenu Presets` mod under the `Stock List [NoDelete]'s` separator of MO2 if you want to ensure they are saved after an update.

## Removing the Modlist

Simply delete the Apostasy folder. Congratulations, you have uninstalled Apostasy.

## Issues

Please check the [FAQ](https://github.com/Oghma-Infinium/Apostasy/blob/main/Documentation/FAQ.md) first if you have any issues.

>[!TIP]
>If you encounter any bugs or issues while playing the list, the [Waking Dreams](https://discord.gg/4WwqfK5yHg) support server is preferred and will have the fastest turn around time for support.  Alternatively, you can leave an issue report on the Github [Issues Page](https://github.com/Oghma-Infinium/Apostasy/issues).

## Credits and Thanks

- *YOU* for reading this.
- [Bingus](https://next.nexusmods.com/profile/bingusthecatto/about-me) for [Ascensio](https://github.com/Oghma-Infinium/Ascensio), ENB tweaking, asset editing, and much, much more.
- Curly for the original iteration of Ascensio that got me started with my first modlist.
- [Ylikollikas](https://next.nexusmods.com/profile/Ylikollikas) for a lot, I can not even begin to list what he has contributed.
- [iAmMe27](https://ko-fi.com/iamme27) for general modding, documentation, and WJ assistance.
- The [Waking Dreams](https://discord.gg/4WwqfK5yHg) Helpers for their time and effort playtesting, providing feedback, and support assistance.
- Those who play tested and provided feedback during beta.
- [Jolly Co-Operators](https://discord.gg/jolly-coop) and [Cacophony](https://www.patreon.com/cacophony1979) for their wonderful community that inspired me to start modding more.
- [JustThatKing](https://next.nexusmods.com/profile/JustThatKing/about-me), [jdsmith2816](https://next.nexusmods.com/profile/jdsmith2816/about-me), and [Total](https://github.com/NotTotal) for their feedback and assistance when I started modding.
- Bethesda Game Studios for Skyrim and the Creation Kit.
- [ElminsterAU](https://www.patreon.com/ElminsterAU) and the xEdit team for SSEEdit.
- [Noggog](https://www.nexusmods.com/skyrim/users/862590) for Mutagen and Synthesis.
- [Halgari](https://www.nexusmods.com/skyrimspecialedition/users/17252164) and the WJ Team for the amazing platform that is Wabbajack.
- [LivelyDismay](https://github.com/LivelyDismay) and [The Animonculory](https://github.com/The-Animonculory) for their modding guides.
- [Sheson](https://ko-fi.com/sheson) for [DynDOLOD](https://dyndolod.info/) and associated tools.
- [Styyx](https://github.com/Styyx1) for assisting heavily in creating DLLs for the custom mods made for the list.
- [Aelarr](https://www.nexusmods.com/skyrim/users/6843757) and Anreme for permissions to use some custom mods from The Owl Archives server.
- Mgde12, D1Z4STR, 半蔵 内倉, Kepler, Hencoat, nostalgic.wave, EnragedHamster, unclemestor, snowpeachcherry, Charlie Kriech, Durgenage, Pacifist Fist, Don Maker, Russell Collins, Oresh, Danimals, Monko, Anehum, hildocean, The Unattested Wombat, Ola Nordman, Regista433, Jaron Scotland, King_Sheogorath, TheRyge, Shakes, highchae, Robbie, cowbellhero55, Geero, JAYDENCITO, Nehellena, Mysthey, Echo, Scott MacLeod, Exanima, Thundertube, LELUGOLELU, ravenlake, Paultinich, icaruscien, Oracraen, Lykk3, VillainousJ, Micheal Hamm, netwolff, Nico, G1Broheim, sweeper240, calcteacher, Ark, Zenity for support on [patreon](https://www.patreon.com/aljoxo).
- adorion1981, aexilkv, AlphaGhost47, ambo, Ananta, annakins, Atlas, Blade, BlueBeagle, Bubborus, Chef Nicnaq, Danimals, derbaer, derkaenaz, DevZan, Don Maker, doombot117, E2J, Elendil, EnragedHamster, FalseRealism / Shingee Tingee, Felivath, Forsaken Jing, freshr, FutureWorld, Gous, Gremlin, hedich, Hencoat, Jeremy, Joey, JoeyFlow, JollyTheRancher, JXEYES, Kannon555, kanpeki, Kathie Murphy, Kiqing, Lunaros, Maelstrom, Mgde12, Mike, Monko, netwolff, orca, paulogrupp, Psyguyy, rezthe0one, Roxiie, SaddestNoddles, shallow_green, skylion, Soloist, Steve, Stryn, thefrogwithnoname, Thomas Brack, Tom Curran, tyler, tyrotoxism, Victoriam, Won Pham, WoWZaton, Xtremza, Zhijia, and zidan for their support via [Ko-fi](https://ko-fi.com/aljoxo).
