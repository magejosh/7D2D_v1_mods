# mjSetBiome

Provides a template settings file that uses XPath to allow users to configure the desired biome settings you desire to play with.

## Features

* Change the desired settings in the blocks.xml file to enable and configure the desired features.

## Dependent and Compatible Modlets

**This modlet requires version `1.0 (b333) or higher` of the base game only, no other mods are required.**

## Technical Details

This modlet uses XPath to modify XML files, and does not require C#.

After installation, **you absolutely must start a new game!**

If you load up an existing game after installing this modlet,
**it will become corrupted and you will lose the game world.**

Here are the details about configuring all this in the XML files.

#### Feature configuration biomes XML
Simple edit the biomes.xml to your desired settings, by editing the values inside the 3 main nodes that are set.

## Credits
Most of this `README.md` was written by khzmusic for his Food Spoilage mod and used here for clarity and ease of production. You will be able to find that mod here when he releases it for greater details about that feature specifically: https://gitlab.com/karlgiesing/7d2d-1.0-mods
