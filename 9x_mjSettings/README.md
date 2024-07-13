# mjSettings

Provides a template settings file that uses XPath to configure the desired 0-SCore and NPCmod settings you desire to play with.

## Features

* Change the desired settings in the blocks.xml file to enable and configure the desired features.

## Dependent and Compatible Modlets

**This modlet requires version `1.0.18.2207` of the `0-SCore` modlet.**
Earlier versions will not work!
You can find 0-SCore here: https://github.com/SphereII/SphereII.Mods/tree/1.0e

## Technical Details

This modlet uses XPath to modify XML files, and does not require C#.

However, the `0-SCore` modlet **does** require C# code.
It is *not* compatible with EAC.

Additionally, this modlet contains new assets (icons).
It must be installed on both clients and servers.

After installation, **you absolutely must start a new game!**

If you load up an existing game after installing this modlet,
**it will become corrupted and you will lose the game world.**

Here are the details about configuring all this in the XML files.

#### Feature configuration block XML
SphereII created a block in `blocks.xml` that is designed to hold feature configuration data
for the entire Core modlet.
Each property node in that block is devoted to one feature, and that node has child property nodes
that hold the configuration data.

### Roadmap
As of SCore Version 1.0.15.1402 and going forward this modlet will match its version numbers on future updates with SCore to make easy identification of compatibility more transparent and intuitive for users.
Intention is to expand the details in this README to include tips and tricks for using SCore as well as explanation of the various features and NPCmod when it releases.

## Credits
Most of this `README.md` was written by khzmusic for his Food Spoilage mod and used here for clarity and ease of production. You will be able to find that mod here when he releases it for greater details about that feature specifically: https://gitlab.com/karlgiesing/7d2d-1.0-mods
