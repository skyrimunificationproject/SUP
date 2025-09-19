![](https://raw.githubusercontent.com/skyrimunificationproject/SUP/main/images/Banner.png)

<p align="center>
[ <a href="https://www.nexusmods.com/skyrimspecialedition">Nexus</a> |
Installation |
<a href="https://github.com/skyrimunificationproject/SUP/blob/main/GAMEPLAY.md">Gameplay Guide</a> |
<a href="https://github.com/skyrimunificationproject/SUP/blob/main/CHANGELOG.md">Changelog</a> |
<a href="https://loadorderlibrary.com/lists/skyrim-unification-project">Load Order</a> |
<a href="https://github.com/skyrimunificationproject/SUP/blob/main/FAQ.md">FAQ</a> |
<a href="https://skyrimunificationproject.github.io/">Modlist Details and Manual Installs</a> ]
</p>

---

**Modlist Support: [Skyrim Unification Project](https://discord.gg/UAhtyb2XuK)**

>[!IMPORTANT]
>Skyrim Unification Project requires the four free AE mods (Fishing, Rare Curios, Survival Mode, and Saints and Seducers) included in the Skyrim Anniversary Edition update from November 2021. This modlist does **NOT** utilize the AE DLC, only these four free AE mods are used.

>[!WARNING]
>You must update Skyrim to the latest version (1.6.1170) on Steam to install this list.

<header>
    <h1>Contents</h1>
</header>

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
    - [Installing Creation Club Files](#installing-creation-club-files)
  - [Wabbajack Installation](#wabbajack-installation)
    - [Installing Wabbajack](#installing-wabbajack)
    - [Downloading and Installing Skyrim Unification Project](#downloading-and-installing-sup)
  - [Problems with installation](#problems-with-installation)
    - [Missing Manual Downloads](#missing-manual-downloads)
- [Post-Installation and Optional Setup](#post-installation-and-optional-setup)
  - [Game Folder](#game-folder)
  - [Antivirus Exceptions](#antivirus-exceptions)
  - [Post-Installation Issues and Troubleshooting](#post-installation-issues-and-troubleshooting)
  - [Keyboard Keybinds](#keyboard-keybinds)
  - [Gamepad Keybinds](#gamepad-keybinds)
- [Playing the List](#playing-the-list)
  - [Before Launching the Game](#before-launching-the-game)
  - [Actually Playing the Game](#actually-playing-the-game)
- [Updating the modlist](#updating-the-modlist)
- [Removing the Modlist](#removing-the-modlist)
- [Issues](#issues)
- [Credits and Thanks](#credits-and-thanks)

# Introduction

Skyrim Unification Project is a modular modlist for *The Elder Scrolls V: Skyrim Special Edition* that allows the player to create their ideal experience. Whether with a framework to build upon, choosing between the different modules offered, or installing everything, the experience will be engaging, consistent, challenging, rewarding, and hassle-free.

Consistency is an essential mission for Skyrim Unification Project, which sets it apart from other mod packs on top of its large scope. Skyrim Unification Project includes thousands of mods that countless talented mod authors provide. These mods are patched and tweaked to ensure a seamless, consistent, and bug-free experience.

Skyrim Unification Project is built around Skyrim Unification Project - Gameplay Overhaul, which was developed alongside the modlist to ensure every mod, whether it is new armor, weapons, clothing, items, quests, enemies, and much more, are patched to create a unified and ultimately cohesive experience.

A full list of the mods used in this modlist can be viewed [here](https://loadorderlibrary.com/lists/skyrim-unification-project).

You can find a summary of all relevant gameplay changes and notable mods on the [Gameplay Guide](https://github.com/skyrimunificationproject/SUP/blob/main/GAMEPLAY.md).

This Wabbajack contains the "Full" install with every available module already enabled and patched for in generated outputs.  Support is only provided for this configuration, but users are free to use different combinations of the modules and utilize the unofficial helpdesk channel.

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

## System Requirements

Based on both internal performance testing and user feedback, the section below outlines my *recommended* system specifications for the list. Please keep in mind that every PC is different, and these recommendations are an estimate based on available data and firsthand reports. Individual performance may vary depending on specific hardware and software configurations, as well as other system optimizations. **Troubleshooting & support for hardware related issues will not be provided.**

>[!WARNING]
>
>- An SSD is **required** to the play the modlist.
>- Only Windows 10 or 11 operating systems are supported. Windows LTSC, special variants, lightened editions or any other modified variant **WILL NOT WORK.** Linux installations also **WILL NOT WORK**.


# Installation

Installing Skyrim Unification Project is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#updating-the-modlist).

## Pre-Installation

These steps are only required for installing the modlist for the first time. Additionally, many of these steps may be covered in other modlist installs, for new users I suggest reading through here regardless.

### Installing Microsoft Visual C++ and .NET

 1. Install [Visual C++ x64](https://aka.ms/vs/17/release/vc_redist.x64.exe).
 2. Install [.NET Runtime 9.X.X Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/9.0).
 3. Install [.NET 6.0 Runtime Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.30-windows-x64-installer).

>[!WARNING]
>If you already have Visual C++ installed, please make sure you install it again and use the `Repair` option to get the latest version of the redistributables. **Do NOT skip this step or MO2 and the game may fail to launch.**

### Pagefile and Crash Prevention

>[!WARNING]
>Larger Skyrim modlists require a significant amount of memory, running out of memory **will** result in crashes and other potential issues. Due to Skyrim Unification Project's size and number of files, this step is **NOT** optional. I do not care how much RAM or VRAM you have, please do this step.

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



### Setting Shader Cache Size (NVIDIA Users Only)

>[!IMPORTANT]
>For NVIDIA users, it is recommended to boost the size of the shader cache. These settings have been shown to improve stability, while it may not be entirely necessary, it is still recommended.

**To do this:**

- Right-click on your desktop and select `NVIDIA Control Panel`
- Navigate and click `Manage 3D Settings`
- Scroll down the **Global Settings** tab until you see **Shader Cache Size**
- Double-click `Driver Default` to the right of **Shader Cache Size** and select `10 GB`
- Click `Apply` in the bottom right hand corner
- Exit out of the application


### Steam Setup

>[!WARNING]
>If you have your Steam Library in Program Files, read [this article](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) by LostDragonist. Locations such as Desktop, Documents, Downloads, OneDrive, etc. *will* cause issues with installing and playing the list.

 1. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
 2. Right click on Skyrim SE and click on properties, untick the `Enable Steam Overlay while in-game.`
 3. Please ensure you follow the steps outlined in the [Installing Creation Club Files](#installing-creation-club-files) section. **DO NOT SKIP THIS STEP OR YOUR INSTALL WILL FAIL.**

### Changing the Game Language

>[!WARNING]
>**The English Steam version of Skyrim SE is the only supported version.**

I understand that this may be frustrating for non-English speaking users or users with the GOG/Bethesda.net versions, but due to the core file differences between the different versions, I am only able to support one game version.

To change your Skyrim SE's language:

 1. Right click on Skyrim SE in Steam
 2. Click `Properties`
 3. Click `Language`
 4. Set the Language to `English`

### Installing Creation Club Files
>
>[!WARNING]
> ***Do NOT skip this step or your install may fail!***

Since the 1.6.1130 update (January 17, 2024), Steam has begun including the free Creation Club (CC) files with the base installation of Skyrim. However, these files do not have the same file hash as the files that are downloaded from the in-game **Creations** menu for Anniversary Edition (AE) users. In order to comply with Wabbajack policy and minimize issues for users who own the AE update, Skyrim Unification Project is compiled using the versions of the CC content that are obtained from the in-game **Creations** menu.  

As a result of this, for users who do not own the AE, you must ensure that you download the correct version of the CC files. Steps below:

 - Navigate to your Skyrim SE's Steam Data folder
    - i.e. `D:\SteamLibrary\steamapps\common\Skyrim Special Edition\data`
 - Delete *both* Rare Curios files:
    - `ccbgssse037-curios.bsa`
    - `ccbgssse037-curios.esl`
 - Launch Skyrim SE from Steam and select **Creations** at the main menu
 - Select **Search** at the bottom and search for `Rare Curios`
 - Select the card titled `Rare Curios` and press **Download**
 - Once it is done, accept Bethesda's load order message and exit the game

>[!IMPORTANT]
>
>- **DO NOT** Alt+Tab during this process or it will fail to properly download these files.
>- **DO NOT** verify your game files after doing the steps above as it will revert the "correct" file hashes for the CC files you downloaded in this step.


## Wabbajack Installation

### Installing Wabbajack

Once you have completed the pre-installation section, follow these steps to install Wabbajack:

1. Create an empty folder named `Wabbajack` on the root of your drive, such as `C:\Wabbajack` for example.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), in your Skyrim's Steam folder, or in any folders related to the modlist itself (the downloads or install folder).**
    > - The `Wabbajack` folder does not need to be on an SSD, but it makes installing faster. You can set this location to be on an HDD for the sake of saving space.

2. Download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases/latest/download/Wabbajack.exe) and place the `Wabbajack.exe` file inside the Wabbajack folder you created in Step 1.

3. Double-click the `Wabbajack.exe` file that is now inside your Wabbajack folder to set up the program.

>[!IMPORTANT]
>The list requires Wabbajack version **4.0.0.0 or later**. Installing the modlist on older versions of Wabbajack will result in issues.

### Downloading and Installing Skyrim Unification Project

>[!CAUTION]
>**A legal copy of Skyrim Special Edition is required.** Pirated copies of the game will cause the installation to fail and even if you manage to somehow get around Wabbajack's built-in piracy prevention measures, SKSE does not work with the cracked exes.  

Downloading and installing Skyrim Unification Project can take a while depending on your internet connection, PC specs, and if you have Nexus Premium. Without Premium, you will need to manually click the **Slow Download** button for each mod.

To install Skyrim Unification Project, complete the following steps.

 1. Open Wabbajack and click `Browse Modlists`
 2. Pick the **Skyrim Special Edition** option from the game filter drop-down box (or use the search bar to find the modlist).
 3. Press the download arrow on the Skyrim Unification Project UI card and wait for it to download
 4. Set the `Modlist Installation Location` to a folder such as `C:\Skyrim Unification Project\`.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), or in your Skyrim's Steam folder**
    > - The `Resource Download Location` does not need to be on an SSD, but it makes installing faster. You can set this location to an HDD for the sake of saving space.
 5. Download the files from the [Missing Manual Downloads](#missing-manual-downloads) section and place them in your designated `Resource Download Location` folder.
 6. Press the play arrow to begin.
 7. Turn on your favorite show or a nice long video essay as Wabbajack does its thing. Alternatively read through this readme again.
 8. If the installation is successful, then rejoice and move onto [post installation](#post-installation-and-optional-setup). If the installation is unsuccessful, follow the tips below or the [discord server](https://discord.gg/UAhtyb2XuK) for support.

## Problems with installation

It is possible that you may encounter an error with Wabbajack when installing. Some common issues are listed below.

<Details>
<summary>I'm having trouble downloading Non-Nexus files or specific files!</summary>

Big files can fail to download due to connection issues or website issues. You can either run Wabbajack again or download the missing file manually. If you decide to manually download the file, make sure to place the file(s) inside the folder you set as the `Resource Download Location`.

This issue can also occur with files sources from Google Drive, MEGA, Patreon, and other sites. Missing Manual Downloads are listed [here](#missing-manual-downloads).

</Details>

<Details>
<summary>Wabbajack couldn't find my game folder!</summary>

Either buy the game or re-read the [Pre-Installation](#pre-installation) section.  

</Details>  

<Details>
<summary>Unable to download 'Data_ccbgssse037-curios': </summary>

Please make sure you are following the steps outlined in the [Installing Creation Club Files](#installing-creation-club-files) section

</Details>  

<Details>
<summary>Unable to download Skyrim_Default.ini or SkyrimPrefs.ini:</summary>

This error means you failed to follow this Readme. Go back and follow the steps outlines in the [Changing the Game Language](#changing-the-game-language) section

</Details>  

<Details>
<summary>Could not find part of the path "TEMP_BSA_FILES"</summary>

This is typically caused by a problem extracting zip files.  

The quickest solution is as follows:  
 1. Close Wabbajack.
 2. Go to your install folder and locate the `TEMP_BSA_FILES` folder (if it exists).
 3. Delete that folder (if it exists).
 4. Restart Wabbajack.
 5. Restart the modlist installation.  

If the `TEMP_BSA_FILES` folder does not exist, then delete the download file for the mod being referenced before restarting Wabbajack.  

**Note**: Using the retry button will not work as Wabbajack does not understand that there was an issue with extraction and will not retry extraction steps.

</Details>  

<Details>
<summary>My antivirus reports a virus with the program or modlist!</summary>

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
 2. Click the **Settings** button in the bottom left corner of the Wabbajack window.
 3. Under the **Performance** box, lower each number for each category to half of what it is currently set.
 4. Continue Installation.

>[!TIP]
> It is suggested to have a program installed on your PC that can open `.json` files, like [Notepad++](https://notepad-plus-plus.org/) or [Visual Studio Code](https://code.visualstudio.com/)

</Details>  

### Missing Manual Downloads

Wabbajack frequently has trouble downloading mods hosted on sites other than Nexus. If you get an error such as **Missing Manual Downloads**, then read this section. You will need to manually download these files and place them in the `Resource Download Location` that is made in the [Downloading and Installing Skyrim Unification Project](#downloading-and-installing-apostasy) section.

>[!WARNING]
> Make sure that you **DO NOT** unzip these files at all.

Google Drive Files:

- [High Poly Head v1.4 (SE)](https://drive.google.com/uc?id=15_0njBUjHKidNnJPmLXEygzGVWsA3Zbq&export=download)



# Post-Installation and Optional Setup

## Game Folder

Skyrim Unification Project uses a Wabbajack feature called Stock Game to keep your Skyrim installation clean. All the files that you need to run the list are in a folder called `Stock Game`. You don’t need to copy anything at all.

## Antivirus Exceptions

>[!WARNING]
>Antivirus programs are notorious for false flagging [MO2's Virtual File System](https://stepmodifications.org/wiki/Guide:Mod_Organizer/Advanced), which can and will cause crashes and other problems. Antivirus programs like BitDefender, Norton, and Webroot are especially aggressive, and you will need to fully remove them from your PC in order to actually launch the game through MO2. It is 2024, Windows Defender and being smart online is more than adequate to protect yourself from malicious software.

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

## Post-Installation Issues and Troubleshooting

<Details>
<summary>Game is zoomed into the top left corner!</summary>

Windows Scaling can prevent games from displaying correctly, and will often result in the game appearing "zoomed in". To fix this, find the `SkyrimSE.exe` located in your `[Path to Modlist]\Stock Game` and follow the steps in the images below:

![](https://raw.githubusercontent.com/SkyrimUnificationProject/SUP/main/images/skyrim-scaling.png)

</Details>

<Details>
<summary>Form 43 Error in MO2. / A DLL plugin has failed to load correctly.</summary>

Your installation is corrupt. Rerun Wabbajack and make sure to tick the **Overwrite Installation** box. If the error persists after a reinstall, then delete the `[Path to Modlist]\mods` folder, and rerun Wabbajack again.

</Details>  

<Details>
<summary>Crashing on Startup</summary>

Create a thread in the `#help-desk` channel of the [discord](https://discord.gg/UAhtyb2XuK), including all relevant crashlogs. There are several reasons why this might happen, and 99.9% of them are a corrupt installation.

</Details>  

<Details>
<summary>Crashes during Gameplay</summary>

Skyrim is a notoriously buggy game and cramming thousands of mods into it is not gauranteed to always produce the most stable experience possible. Especially in heavier lists where you may be pushing the limitations of your hardware as a result of Skyrim's old and unoptimized rendering pipeline.

If you find yourself crashing, then create a thread in the `#help-desk` channel of the [discord](https://discord.gg/UAhtyb2XuK).

In order to get the best possible response please ensure that:

 1. Your crash is reproducible.
 2. You include all relevant crashlogs (if you do not know where to find them then use the `!crashlog` command in chat).
 3. Provide details about the crash (what you were doing, where it took place, if there was an associated quest, etc). Details are necessary in order to quickly diagnose crashes.

</Details>  



## Keyboard Keybinds

You can review the default keybinds in game by pressing `F11`.

## Gamepad Keybinds

>[!WARNING]
>Gamepads may need additional setup in order to work as intended. Please refer to the [Configuration](https://github.com/SkyrimUnificationProject/SUP/blob/main/Documentation/CONFIG.md#gamepad-support) page.


# Playing the List

>[!WARNING]
>Before starting the list, read over the [Configuration](https://github.com/SkyrimUnificationProject/SUP/blob/main/Documentation/CONFIG.md), [FAQ](https://github.com/SkyrimUnificationProject/SUP/blob/main/Documentation/FAQ.md), and [Gameplay](https://github.com/SkyrimUnificationProject/SUP/blob/main/GAMEPLAY.md) pages.

## Before Launching the Game

 1. Head over to your modlist installation folder (e.g. `C:\Skyrim Unification Project`), locate an executable named `ModOrganizer.exe`, and launch it. Your first launch of Mod Organizer 2 may take several minutes due to GitHub repository downloads, so please be patient.


## Actually Playing the Game

 1. Before Launching the game, read over the [Gameplay Guide](https://github.com/SkyrimUnificationProject/SUP/blob/main/GAMEPLAY.md).
 2. Launch the "SKSE" Executable in MO2. The game may take several minutes to load on your first launch. Please be patient and **DO NOT** click the `Unlock` button on the MO2 prompt.
 3. Select the **New Game** button.
 4. Create your character. All presets should default to High Poly Head settings in RaceMenu.
 5. **(OPTIONAL)** Refer to the different MCM options listed on the [Configuration](https://github.com/SkyrimUnificationProject/SUP/blob/main/Documentation/CONFIG.md#in-game-mcm-options) to adjust any MCM settings you'd like.
 6. Talk to the Statue of Mara and pick a start option. While you can do the vanilla intro "Got caught crossing the border", generally the vanilla-adjacent start "Camping in the woods" is recommended for a new player. If you are a veteran player, feel free to choose any option. You can also choose "I am the Guild Master of the Dragonborn Museum" for the special LOTD start (bypasses some content), or "Arrived by boat/Solitude" and accept the prompt when you arrive to become the museum Relic Hunter (no LOTD content skipped).
 7. Sleep on the bed to begin.

# Updating the modlist

Versioning for the list will adhere to the following format: `MAJOR.MINOR.PATCH`.

- `MAJOR`: Any release with a number change here will be considered a major update as at least 1 area of the list was massively overhauled. These updates with **NEVER** be save safe.
- `MINOR`: Any release with a number change here will be considered a minor update, these updates will **not** be save safe, unless otherwise specified.
- `PATCH`: Any release with a number change here will be considered a patch, these updates should be save safe and will be used primarily for bugfixes.
- In some rare cases, a fourth number will be used to designate a `HOTFIX`. These will only be utilized in cases where the list is recompiled with no other changes.

Updating is like installing the list. Simply make sure your paths are the same and tick the `overwrite installation` button. Please keep in mind any mods you have added will be deleted when updating. To make sure that Wabbajack does not delete your added mods upon updating, prefix your mods with `[NoDelete]`.

>[!IMPORTANT]
>Saves can be continued across **Save-Safe** updates. Updates will be indicated whether or not they are **Save-Safe** on the [Changelog](https://github.com/SkyrimUnificationProject/SUP/blob/main/CHANGELOG.md). It is suggested that you backup your saves before updating if you plan on continuing them.


# Removing the Modlist

Simply delete the Skyrim Unification Project folder.

# Issues

Please check the [FAQ](https://github.com/skyrimunificationproject/SUP/blob/main/FAQ.md) first if you have any issues.

>[!TIP]
>If you encounter any bugs or issues while playing the list, please visit our [Skyrim Unification Project](https://discord.gg/UAhtyb2XuK) support server.

# Credits and Thanks

- [Aljo](https://github.com/aljoxo) for permission to use Apostasy's README template.
- Everyone who participates in playtesting and provides feedback during development builds.
- Bethesda Game Studios for Skyrim and the Creation Kit.
- [ElminsterAU](https://www.patreon.com/ElminsterAU) and the xEdit team for SSEEdit.
- [Noggog](https://www.nexusmods.com/skyrim/users/862590) for Mutagen and Synthesis.
- [Halgari](https://www.nexusmods.com/skyrimspecialedition/users/17252164) and the WJ Team for Wabbajack.
- [LivelyDismay](https://github.com/LivelyDismay) for giving a lot of assistance when setting up Wabbajack.
- [Sheson](https://ko-fi.com/sheson) for [DynDOLOD](https://dyndolod.info/) and associated tools.

