# mjFireDanger

![I'm in danger Ralph](https://media.tenor.com/sj0E0izDFH0AAAAM/im-in-danger-ralph.gif)

Enables expanded dangers from 0-SCore and gupFireMod Fire features.

![This is fine](https://media.tenor.com/MYZgsN2TDJAAAAAM/this-is.gif)

## Features

* console logging for fire blocks proximity.
* proximity to fire causes dehydration and if near enough fire will set your clothes on fire too causing you to take burning damage and need to drink water or submerge in water completely to put it out.

## Dependent and Compatible Modlets

**This modlet requires version `1.0.1.1224` of the `0-SCore` modlet.**
Earlier versions will not work!
You can find 0-SCore here: https://github.com/SphereII/SphereII.Mods/tree/1.0e
Also requires [Guppycur](https://community.7daystodie.com/profile/3865-guppycur/)'s Fire Mod, which you can find here: https://community.7daystodie.com/topic/32799-guppy-mods-a21/

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
Ideally I come in and add more note about the SCore fire features and how to adjust them, including alt particles and settings by material and specific block names.
Up next is a CVar for the fire prox logging and an item to toggle it from 1-to-0 so i can turn it on and off in game.

## Credits
Most of the formatting for this `README.md` was written by khzmusic for his Food Spoilage mod and used here for clarity and ease of production. You will be able to find that mod at the following link when he releases it for greater details about that feature specifically: https://gitlab.com/karlgiesing/7d2d-1.0-mods
