
![](https://raw.githubusercontent.com/reyqune/Baldur-s-Gate-3-Enhanced-Edition/refs/heads/main/images/Banner.png)

<p align="center">
  [ <a href="https://ko-fi.com/reyqune">Ko-fi</a> ]
</p>

---

**mod list Support: [reyqune's discord server](https://discord.gg/ty62eQTdkE)**

>[!IMPORTANT]
> Basic reading comprehension is needed to fully enjoy the game.<br/>
> The game folder needs to be clean before you install/play the mod list, and the game needs to be set to English in Steam/GOG, so either fully remove the game and reinstall it, or manually remove any files that do not belong there.<br/>
> The modlist will purge any modded content stored in the AppData folder. Keep this in mind if you have any modded setups through the base game, as they will be removed.<br/>
> Do not have the Baldur's Gate 3 Toolkit installed<br/>

## Introduction

Breathes new life into the realms with improved quality of life, vanquished bugs, enriched visuals, and finely tuned combat balance — all forged with reverence for the spirit of the original adventure.


What the list is:

[Load Order Library page](https://loadorderlibrary.com/lists/baldur-s-gate-3-enhanced-edition)

- Quality of life additions for the user interface to make the experience smoother, also includes multiple options for several different Aspect ratios, 16:9, 16:10, and Ultrawide are available to choose from in Mod Organizer 2. Also includes accessibility options.
- Enriched visuals that makes the world become more alive, but also with several options for personal preference.
- Qualiy of Life additions for the gameplay that makes it overall less tedious, but without deviating too much from the original experience, or breaking the game balance.
- Bug fixes to resolve several issues that still remain in the game even in Patch 8
- Overhauls to gameplay that makes the gameplay more balanced, both with nerfs, and buffs for both the player characters, and the enemies.
- Even though the list was built to be played at Tactician+, you can also play it at any other difficulty level too.
- Minor overhauls to a few story elements to make them smoother
- A template to use to build a mod list of your own based on, the mods are clearly categorised.
- The modlist has several options to customise the experience for your needs, there are options to make the difficulty higher, or lower using the different options provided. Most of these are set to the game's default settings by default, but can be changed by you the player. Overall difficulty can be customised thanks to the Tacitician Enhanced Mod, which by default scales the difficulty based on the setting you choose for the configurable party size mod, it is set to 4 by default, but can be increased/decreased using the MCM. But there are also some other elements which can be customised for prefered difficulty.

What the list isn't:
- additional races/classes
- changes that deviate way too much from the original experience designed by Larian
- adult mods, or frameworks
- a kitchen sink of every mod available on nexusmods, mashed together into one strange cursed mix
- cheats, unbalanced content, too punishing content, or too easy content. (Or rather that all depends on your skill as a player obviously ;))
- a list to play regular honour mode, use custom mode instead. There are too many issues to break the game without mods, and it's unpredictable how these mods will affect a genuine honour mode play-through.


A full list of the mods used in this mod list can be viewed [here](https://www.wabbajack.org/search/BG3EE/BG3EE)

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

### System Requirements

**I will not provide troubleshooting or support for hardware related issues.**

>[!WARNING]
>
>- An SSD is **required** to the play the modlist.
>- Only Windows 10 or 11 operating systems are supported. Windows LTSC, special variants, lightened editions or any other modified variant **will not work.** Linux installations may work, but aren't supported, see the instructions bellow, or click [here](#Linux) for how to install. MacOS is just fully unsupported.

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

## Installation

Installing the mod list is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the mod list, you can safely skip to the [updating section](#updating-the-mod list).

>[!WARNING]
>
> You have to either install the mod list to the same drive where the game is installed, or set the root builder in the included mod organiser 2 to copy post-install.

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

Uninstall the Baldur's Gate 3 Toolkit

Uninstall the game completely, delete anything left of the install folder (e.g. `C:/Steam/steamapps/common/Baldurs Gate 3`), and delete the folder at `%Localappdata%\Larian Studios`. This is to ensure that no errant files are left over from any previous playthroughs and is especially important for preventing data mismatches that will block multiplayer. Cleaning everything improves the odds that the modlist works as expected by providing a blank slate to build up from. Otherwise some files like an unwanted modsettings.lsx or gustavdev could interfere with the mod list. This is especially important now with Mod.io integration and Larian's official mod manager services.

Install the game through Steam/GOG, and launch it at least once, and then quit via the main menu of the game.

#### Changing the Game Language

>[!WARNING]
>**The English version of Baldur's Gate 3 is the only supported version.**
> Other versions MAY work, but will end up being a combination of that language, and partially English.

To change your Baldur's Gate 3's language:
Steam:
 1. Right click on Baldur's Gate 3 in Steam
 2. Click `Properties`
 3. Click `Language`
 4. Set the Language to `English`
GOG:
https://support.gog.com/hc/en-us/articles/4412958845329-How-do-I-change-the-game-language

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
 
 The modlist has several optional mods that can be toggled on/off inside the included mod organizer software.
 
 For a better gameplay experience, it's recommended to disable the Karmic Dice
 1. Open the settings, and go to the Gameplay section
 2. Toggle Karmic Dice off
 3. Press Save
 ![](https://raw.githubusercontent.com/reyqune/Baldur-s-Gate-3-Enhanced-Edition/refs/heads/main/images/karmicDice.jpg)
 
 ### Starting a new campaign
 
To play the modlist at the intended difficulty level, you need to start a new game using the Custom Difficulty.
<br/>
When starting a new campaign, navigate to the right to select Custom Difficulty (it's after Honour Mode).
<br/>
<br/>
Hit "Restore Default" at the bottom-right in the Custom Difficulty menu, all options should update to the intended settings.
<br/>
The only exception is that you must manually change the ruleset from Standard Ruleset to Honour Ruleset, at the top of Custom Difficulty.
<br/>
<br/>
Make sure you set this correctly, as you will not be able to change this later.
<br/>
<br/>
While you are free to customise the settings as you prefer them, this is what the modlist was balanced around.

![](https://raw.githubusercontent.com/reyqune/Baldur-s-Gate-3-Enhanced-Edition/refs/heads/main/images/rules.jpg)

### Setting the root builder to copy mode.

 1. Open the bundled mod organiser 2
 2. Click tools
 3. Click root builder
 4. Click on copy
 5. You're done and can now launch the game if it's installed on another drive, but keep in mind that this will copy files to the actual game folder when the game is launched.
 NOTE: Those files will not be automatically removed if the game is exited in an unexpected manner such as if it crashes, or is force closed by the task manager. To resolve that use the clear button.
 
 ![](https://raw.githubusercontent.com/reyqune/Baldur-s-Gate-3-Enhanced-Edition/refs/heads/main/images/root_builder_howto.png)

## Updating the mod list

Versioning for the list will adhere to the following format: `MAJOR.MINOR.PATCH`.

- `MAJOR`: Any release with a number change here will be considered a major update as at least 1 area of the list was massively overhauled. These updates with **NEVER** be save safe.
- `MINOR`: Any release with a number change here will be considered a minor update, these updates will usually not be save safe, unless otherwise specified.
- `PATCH`: Any release with a number change here will be considered a patch, these updates should be save safe and will be used primarily for bugfixes.
- In some rare cases you may see a fourth slot be used, which I will refer to as `HOTFIX`. These list "updates" will be used if the list needs to be recompiled for any reason. There will be no changes in these "updates" as they are purely for maintenance.

Updating is like installing the list. Simply make sure your paths are the same and tick the `overwrite installation` button. Please keep in mind any mods you have added will be deleted when updating. To make sure that Wabbajack does not delete your self-added, mods upon updating, prefix your installed mods with `[NoDelete]`.

## Removing the mod list

Simply delete the mod list folder. Congratulations, you have uninstalled the mod list.

## Linux
(provided as is)

# (Linux) Install Wabbajack
Follow this [guide](https://github.com/Omni-guides/Wabbajack-Modlist-Linux/wiki/Wabbajack-via-Proton) to install Wabbajack via Steam.

# (Linux) Download BG3 Enhanced
Start Wabbajack with your Steam shortcut and Download the list. The download location can be anywhere, but the install location should be on the same disk as BG3.

# (Linux) Configuration of the Mod Organizer 2 prefix
Step 1: Have the modlist downloaded

Step 2: Go to https://github.com/SulfurNitride/NaK, download the latest release.

Step 3: Open the terminal where NaK is located, and run two commands. `chmod +x nak` and `./nak`

Step 4: Choose Mod Managers, MO2, and Setup existing installation.

Step 5: Provide the MO2 folder for the modlist and let it add it to steam and do dependancies.

Step 6: After everything has completed, open up BG3EE and set root builder to copy. 

Step 7: Enjoy the modlist.

Requirements: Protontricks (flatpak, or native), and steam (native only), and Proton Experimental

# (Linux) Configuration of Mod Organizer 2
Rootbuilder needs to be changed from the link mode to copy mode. To do this, click the puzzle symbol -> root builder -> root builder and check the box next to 'copy'. 

# (Linux) Launch the game
Launch the game by choosing BG3 - Vulkan, and click on run.

## Issues

>[!TIP]
>If you encounter any bugs or issues while playing the list, go to the [reyqune's discord server](https://discord.gg/ty62eQTdkE) for help.

## Credits and Thanks

- [*YOU*](https://www.youtube.com/watch?v=1TO48Cnl66w) for reading this.
- [Everyone](https://www.youtube.com/watch?v=74BzSTQCl_c) who contributed to the making of the included mods that are included in this here mod list
- [aljoxo](https://github.com/aljoxo) the [creator of the template](https://github.com/Oghma-Infinium/Apostasy/) for making the readme this document is based on
- The Wabbajack devs for making [Wabbajack](https://github.com/wabbajack-tools/wabbajack)
- [Ajax](https://github.com/ajaxxxxxxxx), and [LillyBird](https://linktr.ee/lillybird69) the creators of the list [Listonomicon](https://www.nexusmods.com/baldursgate3/mods/15237)
- [BaldursGoonsack](https://next.nexusmods.com/profile/BaldursGoonsack/about-me?gameId=3474) the creator of the list [Difficulty, Immersion, Quality](https://next.nexusmods.com/baldursgate3/collections/pns4qv)
- the creator of the plugin that made it possible to mod BG3 in MO2, [Alvadus (zino)](https://github.com/Alvadus)
- steven2137 for writing the Linux guide, and Sulfur Nitride for providing more steps for the linux instructions