
![](https://raw.githubusercontent.com/reyqune/Baldur-s-Gate-3-Enhanced-Edition/refs/heads/main/images/Banner.png)

<p align="center">
  [ <a href="https://ko-fi.com/reyqune">Ko-fi</a> ]
</p>

---

**mod list Support: [reyqune's discord server](https://discord.gg/ty62eQTdkE)**

>[!IMPORTANT]
> Basic reading ability is needed to fully enjoy this game.<br/>
> The game folder needs to be clean before you install/play the mod list, and the game needs to be set to English in Steam, so either fully remove the game and reinstall it, or manually remove any files that do not belong there.<br/>
> The mod list will purge any modded content stored in the appdata folder, keep this in mind if you have any modded setup through the base game. As that will be purged.<br/>
> Do not have the baldur's gate 3 tool kit installed<br/>

## Introduction

A minimalist curated Baldur's Gate 3 mod list that stays (somewhat) true to the vanilla experience but also a bit more difficult, featuring a handful of quality-of-life improvements, and bug fixes for a smoother and more polished gameplay.
The list is meant to be played on the tactician mode difficulty, or higher. But there are options to play on lower difficulty by disabling the mod [Combat Extender](https://www.nexusmods.com/baldursgate3/mods/5207).
It does deviate somewhat in order to have a bit more balance, most of which can be toggled off if you prefer, but I cannot guarantee that any such changes will work perfectly fine, as the list is intended to be played as is.


What is included:
https://loadorderlibrary.com/lists/baldur-s-gate-3-enhanced-edition

- QoL additions and fixes for the UI
- Better CPU performance
- [Camera overhaul](https://www.nexusmods.com/baldursgate3/mods/945)
- Some minor overhauls of the visuals, mostly fixes to minor issues.
- Gameplay changes are mostly QoL changes, and bug fixes to make the overall experience less tedious, and a few balance changes like via the mod [Relative Ability Boost Items](https://www.nexusmods.com/baldursgate3/mods/11057).
- There are a few gameplay changes to increase the overall difficulty via the mod [Combat Extender](https://www.nexusmods.com/baldursgate3/mods/5207)
- Other than that the rest of the changes are bug fixes, or fixes to parts of the game that seemed broken, but weren't technically bugs

What the list isn't:
- [Listonomicon](https://www.nexusmods.com/baldursgate3/mods/8976), you should go play it instead if you want what it provides, say hello to the devs from me. <3
- additional races/classes
- changes that deviate way too much from the original experience designed by Larian
- adult mods, or frameworks
- a kitchen sink of every mod available on nexusmods, mashed together into one strange cursed mix
- cheats, unbalanced content, or too punishing content
- a list to play regular honour mode, use custom mode instead. There are too many issues to break the game without mods, and it's unpredictable how these mods will affect a genuine honour mode play-through


A full list of the mods used in this mod list can be viewed [here](https://loadorderlibrary.com/lists/baldur-s-gate-3-enhanced-edition)

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

### System Requirements

The listed specs are the best idea of a baseline that I can provide at the current moment, based on feedback I have gotten from testers and my own experiences. In the future this will be updated depending on feedback received. Your PC may run the list better or worse due a variety of reasons, **I will not provide troubleshooting or support for hardware related issues.**

>[!WARNING]
>
>- Basic reading ability is needed to fully enjoy this game.
>- An SSD is **required** to the play the mod list.
>- Only Windows 10 or 11 operating systems are supported. Windows LTSC, special variants, lightened editions or any other modified variant **WILL NOT WORK.** Linux installations may work, but aren't supported. MacOS is just fully unsupported.

    Minimum:
        Requires a 64-bit processor and operating system
        OS: Windows 10 64-bit
        Processor: Intel I5 4690 / AMD FX 8350
        Memory: 8 GB RAM
        Graphics: Nvidia GTX 970 / RX 480 (4GB+ of VRAM)
        DirectX: Version 11
        Storage: 150 GB available space
        Additional Notes: SSD required

    Recommended:
        Requires a 64-bit processor and operating system
        OS: Windows 10 64-bit
        Processor: Intel i7 8700K / AMD r5 3600
        Memory: 16 GB RAM
        Graphics: Nvidia 2060 Super / RX 5700 XT (8GB+ of VRAM)
        DirectX: Version 11
        Storage: 150 GB available space
        Additional Notes: SSD required

> The **Install Size** listed on the Wabbajack Gallery is **wrong** and does not properly account of the size saved by compressing files during the installation.

## Installation

Installing the mod list is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the mod list, you can safely skip to the [updating section](#updating-the-mod list).

### Pre-Installation

These steps are only required for installing the mod list for the first time. Additionally, many of these steps may be covered in other mod list installs, for new users I suggest reading through here regardless.

#### Installing Microsoft Visual C++ and .NET

 1. Install [Visual C++ x64](https://aka.ms/vs/17/release/vc_redist.x64.exe).
 2. Install [.NET Runtime 8.X.X Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-8.0.13-windows-x64-installer).
 3. Install [.NET 6.0 Runtime Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.30-windows-x64-installer).

>[!WARNING]
>If you already have Visual C++ installed, please make sure you install it again and use the `Repair` option to get the latest version of the redistributables. **Do NOT skip this step or MO2 and the game may fail to launch.**

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

#### Cleaning a previously installed game setup

Uinstall the Baldur's Gate 3 Tool Kit

Uninstall the game completely, delete anything left of the install folder (e.g. `C:/Steam/steamapps/common/Baldurs Gate 3`), and delete the folder at `%Localappdata%\Larian Studios`. This is to ensure that no errant files are left over from any previous playthroughs and is especially important for preventing data mismatches that will block multiplayer. Cleaning everything improves the odds that the mod list works as expected by providing a blank slate to build up from. Otherwise some files like an unwanted modsettings.lsx or gustavdev could interfere with the mod list. This is especially important now with Mod.io integration and Larian's official mod manager services.

Install the game through Steam, and launch it at least once, and then quit via the main menu of the game.

#### Changing the Game Language

>[!WARNING]
>**The English Steam version of Baldur's Gate 3 is the only supported version.**

To change your Baldur's Gate 3's language:

 1. Right click on Baldur's Gate 3 in Steam
 2. Click `Properties`
 3. Click `Language`
 4. Set the Language to `English`

#### Steam Setup

>[!WARNING]
>If you have your Steam Library in Program Files, read [this article](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) by LostDragonist. Locations such as Desktop, Documents, Downloads, OneDrive, etc. *will* cause issues with installing and playing the list.

 1. Change Baldur's Gate 3 so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
 2. Right click on Baldur's Gate 3 and click on properties, untick the `Enable Steam Overlay while in-game.`
 3. go into Steam\steamapps and [make the file appmanifest_1086940.acf read only](https://support.microsoft.com/en-us/office/make-a-document-read-only-5c25909c-46d9-4eb0-9d1f-d072a560e340) to prevent Baldur's Gate 3 from updating

### Wabbajack Installation

#### Installing Wabbajack

Once you have completed the pre-installation section, follow these steps to install Wabbajack:

1. Create an empty folder named `Wabbajack` on the root of your drive, such as `C:\Wabbajack` for example.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), in your Skyrim's Steam folder, or in any folders related to the mod list itself (the downloads or install folder).**
    > - The `Wabbajack` folder does not need to be on an SSD, but it makes installing faster. You can set this location to be on an HDD for the sake of saving space.

2. Download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases/latest/download/Wabbajack.exe) and place the `Wabbajack.exe` file inside the Wabbajack folder you created in Step 1.

3. Double-click the `Wabbajack.exe` file that is now inside your Wabbajack folder to set up the program.

>[!IMPORTANT]
>The list requires Wabbajack version **3.6.1.0 or later**. Installing the mod list on older versions of Wabbajack will prevent the installation from being completed.

#### Downloading and Installing the mod list

>[!CAUTION]
>**A legal copy of Baldur's Gate 3 is required.**  

Downloading and installing the mod list can take a while depending on your internet connection, PC specs, and if you have Nexus Premium. Without Premium, you will need to manually click the **Slow Download** button for each mod.

To install the mod list, complete the following steps.

 1. Open Wabbajack and click `Browse mod lists`
 2. Tick on the `Show Unofficial Lists` box and pick the **Baldur's Gate 3** option from the game filter drop-down box (or use the search bar to find the mod list)
 3. Press the download arrow on the mod list UI card and wait for it to download
 4. Set the `mod list Installation Location` to a folder such as `C:\modlist`.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), or in your Skyrim's Steam folder**
    > - The `Resource Download Location` does not need to be on an SSD, but it makes installing faster. You can set this location to an HDD for the sake of saving space.
 5. Press the play arrow to begin.
 6. Turn on your favorite show or a nice long video essay as Wabbajack does its thing. Alternatively read through this readme again.
 7. If the installation is successful, then rejoice and move onto [post installation](#post-installation-and-optional-setup). If the installation is unsuccessful, follow the tips below or the [discord server](https://discord.gg/ty62eQTdkE) for support.

### Problems with installation

It is possible that you may encounter an error with Wabbajack when installing. Some common issues are listed below.

<Details>
<summary>Wabbajack couldn't find my game folder!</summary>

Either buy the game, or re-read the [Pre-Installation](#pre-installation) section.  

</Details>  

<Details>
<summary>My antivirus reports a virus with the program or mod list!</summary>

Windows 10/11 may automatically quarantine a key file which is needed for Mod Organizer. You can fix this by [adding an exclusion for Mod Organizer in windows defender](#antivirus-exceptions).  

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

### Antivirus Exceptions

>[!WARNING]
>Antivirus programs are notorious for false flagging [MO2's Virtual File System](https://stepmodifications.org/wiki/Guide:Mod_Organizer/Advanced), which can and will cause crashes and other problems. Antivirus programs like BitDefender, Norton, and Webroot are especially aggressive, and you will very likely need to fully remove them from your PC in order to actually launch the game through MO2. It is 2024, Windows Defender and being smart online is more than adequate to protect yourself from malicious software.

If you use Windows Defender, it is advised that you set up an exception for the mod list.

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

</Details>  

## Playing the List

### Starting the Game

 1. Head over to your mod list installation folder (e.g. `C:\modlist`), locate an executable named `ModOrganizer.exe`, and launch it. Your first launch of Mod Organizer 2 may take several minutes due to GitHub repository downloads, so please be patient.

 4. Launch the "Play" Executable in MO2. The game may take several minutes to load on your first launch. Please be patient and **DO NOT** click the `Unlock` button on the MO2 prompt.
    a. **I REPEAT, DO NOT CLICK THE UNLOCK BUTTON! YOU WILL BREAK YOUR GAME!**
 5. Select the **New Game** button.
 6. Select custom difficulty, and play on tactician difficulty or higher, and choose the other options as you want them to be
 7. Create your lovely character.
 
 ### Optionals
 
 For a better gameplay experience, it's recommended to disable the Karmic Dice
 1. Open the settings, and go to the Gameplay section
 2. Toggle Karmic Dice off
 3. Press Save
 ![](https://raw.githubusercontent.com/reyqune/Baldur-s-Gate-3-Enhanced-Edition/refs/heads/main/images/karmicDice.jpg)

## Updating the mod list

Versioning for the list will adhere to the following format: `MAJOR.MINOR.PATCH`.

- `MAJOR`: Any release with a number change here will be considered a major update as at least 1 area of the list was massively overhauled. These updates with **NEVER** be save safe.
- `MINOR`: Any release with a number change here will be considered a minor update, these updates will usually not be save safe, unless otherwise specified.
- `PATCH`: Any release with a number change here will be considered a patch, these updates should be save safe and will be used primarily for bugfixes.
- In some rare cases you may see a fourth slot be used, which I will refer to as `HOTFIX`. These list "updates" will be used if the list needs to be recompiled for any reason. There will be no changes in these "updates" as they are purely for maintenance.

Updating is like installing the list. Simply make sure your paths are the same and tick the `overwrite installation` button. Please keep in mind any mods you have added will be deleted when updating. To make sure that Wabbajack does not delete your self-added, mods upon updating, prefix your installed mods with `[NoDelete]`.

## Removing the mod list

Simply delete the mod list folder. Congratulations, you have uninstalled the mod list.

## Issues

>[!TIP]
>If you encounter any bugs or issues while playing the list, go to the [reyqune's discord server](https://discord.gg/ty62eQTdkE) for help.

## Credits and Thanks

- [*YOU*](https://www.youtube.com/watch?v=1TO48Cnl66w) for reading this.
- [Everyone](https://www.youtube.com/watch?v=74BzSTQCl_c) who contributed to the making of the included mods that are included in this here mod list
- [aljoxo](https://github.com/aljoxo) the [creator of the template](https://github.com/Oghma-Infinium/Apostasy/) for which this readme is based upon for making the readme this readme is based on which made it easier to make a readme
- The wabberjack devs for making [Wabberjack](https://github.com/wabbajack-tools/wabbajack)
- [Ajax](https://github.com/ajaxxxxxxxx), and [LillyBird](https://linktr.ee/lillybird69) the creators of the list [Listonomicon](https://www.nexusmods.com/baldursgate3/mods/8976)
- [BaldursGoonsack](https://next.nexusmods.com/profile/BaldursGoonsack/about-me?gameId=3474) the creator of the list [Difficulty, Immersion, Quality](https://next.nexusmods.com/baldursgate3/collections/pns4qv)
- the creator of the plugin that made it possible to mod BG3 in MO2, [Alvadus (zino)](https://github.com/Alvadus)
