
![](https://raw.githubusercontent.com/reyqune/Baldur-s-Gate-3-Enhanced-Edition/main/images/Banner.png)

<p align="center">
  [ <a href="https://ko-fi.com/reyqune">Ko-fi</a> ]
</p>

---

**Modlist Support: [reyqune's discord server](https://discord.gg/QjBtu2JA)**

>[!IMPORTANT]
- The game folder needs to be clean before you install/play the mod list, and the game needs to be set to English in Steam

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
      - [Downloading and Installing Apostasy](#downloading-and-installing-the-mod-list)
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

a mostly vanilla plus mod list with the additon of a few quality of life additions, and some visual improvements.
the main focus is to basically be an enhanced edition of the game

A full list of the mods used in this modlist can be viewed on the WJ gallery page

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
>- Only Windows 10 or 11 operating systems are supported. Windows LTSC, special variants, lightened editions or any other modified variant **WILL NOT WORK.** Linux installations may work, but aren't supported.

Minimum requirements:

Processor: AMD r5 3600 (or Intel equivalent)

Memory: 32 GB RAM

Graphics: Nvidia 2080 Super (or AMD equivalent)

<Details>
<summary>Clarification on PC Requirements</summary>

</Details>

Downloads Size: ~14 GB  
Install Size: ~16 GB  
Game:		~143 GB
Temporary Files: ~16 GB (on OS drive)  
**TOTAL:** ~175 GB

> The **Install Size** listed on the Wabbajack Gallery is **wrong** and does not properly account of the size saved by compressing files during the installation.

## Installation

Installing the mod list is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#updating-the-modlist).

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
>Larger modlists require a significant amount of memory, running out of memory **will** result in crashes and other potential issues. Due to the mod list's size and number of files, this step is **NOT** optional. I do not care how much RAM or VRAM you have, please do this step.

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

#### Downloading and Installing the mod list

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

## Playing the List

### Starting the Game

 1. Head over to your modlist installation folder (e.g. `C:\modlist`), locate an executable named `ModOrganizer.exe`, and launch it. Your first launch of Mod Organizer 2 may take several minutes due to GitHub repository downloads, so please be patient.

 4. Launch the "Play" Executable in MO2. The game may take several minutes to load on your first launch. Please be patient and **DO NOT** click the `Unlock` button on the MO2 prompt.
    a. **I REPEAT, DO NOT CLICK THE UNLOCK BUTTON! YOU WILL BREAK YOUR GAME!**
 5. Select the **New Game** button.
 6. Create your lovely character.

## Updating the modlist

Versioning for the list will adhere to the following format: `MAJOR.MINOR.PATCH`.

- `MAJOR`: Any release with a number change here will be considered a major update as at least 1 area of the list was massively overhauled. These updates with **NEVER** be save safe.
- `MINOR`: Any release with a number change here will be considered a minor update, these updates will usually not be save safe, unless otherwise specified.
- `PATCH`: Any release with a number change here will be considered a patch, these updates should be save safe and will be used primarily for bugfixes.
- In some rare cases you may see a fourth slot be used, which I will refer to as `HOTFIX`. These list "updates" will be used if the list needs to be recompiled for any reason. There will be no changes in these "updates" as they are purely for maintenance.

Updating is like installing the list. Simply make sure your paths are the same and tick the `overwrite installation` button. Please keep in mind any mods you have added will be deleted when updating. To make sure that Wabbajack does not delete your added mods upon updating, prefix your mods with `[NoDelete]`.

## Removing the Modlist

Simply delete the mod list folder. Congratulations, you have uninstalled the mod list.

## Issues

>[!TIP]
>If you encounter any bugs or issues while playing the list, the [reyqune's discord server](https://discord.gg/QjBtu2JA) support server is preferred and will have the fastest turn around time for support.

## Credits and Thanks

- *YOU* for reading this.
- Everyone who contributed to the making of the included mods that are included in this here mod list
- The makers of the template for which this readme is based upon for making the readme this readme is based on which made it easier to make a readme
- The wabberjack devs for making wabberjack