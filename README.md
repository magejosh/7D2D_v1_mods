# 7D2D_v1_mods
Mods and modlets (small modifications) for the game 7 Days To Die (aka 7D2D):
[7daystodie.com](https://7daystodie.com/)

I am user [magejosh](https://community.7daystodie.com/profile/51265-khzmusik/) on the 7D2D forums.
I borrowed this README format from user [khzmusik](https://community.7daystodie.com/profile/51265-khzmusik/) on the 7D2D forums.

By convention, modlet authors create new repos for each alpha version of 7D2D.
These modlets were created for, and tested with, **Version 1.0** of the game.

Repos for previous versions are here:

* [Alpha 20 modlets](https://github.com/magejosh/a20NPCmodAdditions)
* [Alpha 21 modlets](https://github.com/magejosh/7d2d_a21_mjMods)

## Installation

> :information_source:
> These mods and modlets are for personal computers only (Windows/Mac/Linux).
> Modding is currently not supported on consoles (XBox/PC).

Each modlet has an individual `README.md` file.
Under the technical details secion, it should tell you whether you need to start a new game
or generate a new world.

But if you want to be safe, generate a new game world after installing *any* modlets.

### Types of mods

For the most part, there are three different kinds of mods:

1. _Modlets_ which use XPath to modify the game's XML configuration files.
    These modlets can be used with EAC.
    In multi-player games, servers will push the XML changes to the client,
    so clients do not need to install the modlet before connecting.
2. Mods which include custom assets (Unity packages, custom icons, etc.)
    usually in addition to using XPath.
    These modlets can be used with EAC.
    However, in multi-player games, servers will **not** push the assets to the client,
    so clients **do** need to install the modlet before connecting.
    > :warning: Mods with custom Unity assets _might not_ work on non-Windows machines.
1. Mods that include custom C# code in a compiled .dll,
    usually in addition to using XPath and/or including custom assets.
    These modlets can **not** be used with EAC, so the game must be launched with EAC turned off.
    In multi-player games, servers will **not** push the .dll to the client,
    so clients **do** need to install the modlet before connecting.

Each individual mod should have its own README.md file,
which will explain whether the mod uses XPath, has custom assets, and/or has custom code.

In addition, many mods are dependent upon other mods being installed.
You will need to install these mod dependencies separately.
Details about the mod's dependencies should also be in the README.md file.

### Installation using the Mod Launcher

Using the Mod Launcher is the recommended way to install these modlets.
In addition to being easier to work with,
it can automatically update any mods it installs.

The Mod Launcher can be downloaded here:

* [7d2dmodlauncher.org](http://7d2dmodlauncher.org)

I recommend creating a new "My Mods" game installation, and installing mods into that;
this keeps the "My Mods" game files completely separate from the vanilla game.

These instructions are for the Mod Launcher version 5,
which is the latest version as of this writing.

To create a new "My Mods:"

1. Ensure you are connected to the Internet.
2. In the Mod Launcher, click on `Install New Mod`.
    The Mod Launcher will download data about the available mods.
    This might take a while, so be patient.
3. In the "Available Mods" screen that appears, click `Add new My Mods`.
4. Enter a name of your choice into the "My Mod Name" field.
    This will end up being a folder name on your system.
5. In the mod-specific page that shows up, there will be a path to the installed game.
    Click the `Clone` button next to it.
    This will copy the game files to the mod's folder
    (by default, `C:\7D2D\Custom\[MyModName]` on Windows).
6. A confirmation dialog will pop up, asking you to confirm you want to copy the game.
    Click `Confirm` to start copying.
7. Once copying is done, click `Manage Modlets`.
8. Use the list on the left to find and install modlets.
9. After you have found and installed the modlets,
    return to the "My Mods" screen,
    and click `Play` to play the game.

### Manual installation into the "vanilla" 7D2D Mods folder

With this method, you will download the source code from the GitLab site,
and move the code directly into your 7D2D game folder.

1. Open the GitLab page for this project:
   
    [https://gitlab.com/karlgiesing/7d2d-a21-modlets](https://gitlab.com/karlgiesing/7d2d-1.0-modlets)

    You can download all the mods at once, or separately,
    by going to each mod's subdirectory.
2. Make sure you are on the master branch (by default, you should be).
3. On the middle right-hand side of the page, below the description, will be a download button;
    click it and select the compression type of your choice (e.g. "zip" for Windows users).
4. Download the compressed file to a directory of your choice.
5. Uncompress the file. This will create a containing folder, for example `7d2d-a21-modlets-master`.
6. Open up your 7D2D game folder.
    On Windows, it is usually located here:

    `%appdata%\7 Days To Die`

    ...where `%appdata%` is a Windows-defined location on your system hard drive.
    For example, on my system, `%appdata%` is located at `C:\Users\[my user name]\AppData\Roaming\`.
    > Note: In A20 and below, this directory was located in the game's directory.
    > Even if supported in 1.0, it will not be supported for very long,
    > so I recommend you do _not_ use this folder.
7. Create a `Mods` folder if one does not already exist.
8. Move any desired mod **subdirectories** from the `7d2d-modlets-master` directory into the game's `Mods` folder.

The next time the game is started, these mods will be active.

### Manual installation into the Mod Launcher's game folder

You should only need to do this if the mod is not (yet) displayed in the mod launcher.
This only applies to *new* mods - updates to existing modlets should be handled automatically.
New mods should automatically show up when merged to the master branch on GitLab,
but there is often a significant delay before they do.

1. Create a new "My Mods" as detailed above, but stop at the `Manage Modlets` step.
    This will create an entirely new game folder (by default, in `C:\7D2D\Custom\[MyModName]`).
2. Download the source code from the GitLab site,
    as you would if you were installing modlets into the vanilla game.
3. In the Mod Launcher, if you're not already on the "Manage Modlets" screen, go there.
4. Click `Manage External Modlets`. An "External Modlets" dialog should open.
5. Click `Open Modlet Folder`.
    This will open the folder on your hard drive where the Mod Launcher stores external modlets.
6. Drag the source code of the modlet, which you downloaded from GitLab, to that folder.
7. If it doesn't show up in the Mod Launcher right away, you may have to click `Refresh`.
8. Once the modlet(s) are displayed, click `Process`.
9. The modlets should now be ready to add to any My Mods for that alpha.

Once the Mod Launcher "catches up" and recognizes the new modlet, you should be able to install
updates automatically, as if you installed them from the Mod Launcher in the first place.

## Mod Versioning

I am adopting something similar to [Semantic Versioning 2.0](https://semver.org/),
except with four numbers rather than three.

Here is what each number means:
1. 7 Days To Die major version (1 in version 1.0) on which the mod was _developed and tested_
2. 7 Days To Die minor version (0 in version 1.0) on which the mod was _developed and tested_
3. Major version of _the mod_ (starting with 1 for the first public release) -
    any changes to the mod that require a new game, _must_ require a new major version
4. Minor (backwards-compatible, non-game-breaking) version of _the mod_

Examples:

* The mod is developed on 7D2D version 1.0.
    This is the first public release of the mod.
    Version:
    ```
    1.0.1.0
    ```
* The mod is developed on 7D2D version 1.0, but 7D2D updates to version 1.1.
    The mod was initially released and is at version 1.0.2.1,
    but it requires changes because of the game update.
    However, if the new alpha doesn't break game saves, installing the new version of the mod
    also will not break game saves.
    New version:
    ```
    1.1.2.1
    ```
* The mod is developed on 7D2D version 1.2.
    The mod was initially released and is at version 1.2.1.0,
    but there is an added feature that will work without starting a new game.
    New version:
    ```
    1.2.1.1
    ```

## Support
The easiest way to contact me is
[through the 7D2D forums](https://community.7daystodie.com/profile/51265-khzmusik/).

If desired, you can also raise an issue in GitLab.

New feature requests are welcome,
but there is no guarantee that I will be able (or willing) to do them.

## Contributing
I would greatly appreciate any help with translations.
I have included translations for the texts in most modlets,
but they were generated through online translation tools,
and probably sound ridiculous to native speakers.

Additionally, any help with testing or balancing is welcome.
I do not play multiplayer games, so reporting any multiplayer bugs is especially welcome.

I may also need help with specific modlets.
If so, I will ask for help in the README.md file of those modlets.

## License
[![License: CC0-1.0](https://licensebuttons.net/l/zero/1.0/80x15.png)](http://creativecommons.org/publicdomain/zero/1.0/)

I hereby dedicate all of these modlets to the public domain.

> :information_source:
> **This license applies only to my own original work.**
> 
> It does _not_ apply to any text, graphics, code,
> or other works created by other people or organizations,
> including any works that I modify in these modlets.
> This applies to any works by The Fun Pimps, other mod/modlet authors,
> or creators of purchased Unity assets.

If I have incorporated or modified the works of any other authors,
they should be credited in the `README.md` file for the modlet which uses those works.
If this is not the case, please let me know, and I will fix this as soon as possible.
