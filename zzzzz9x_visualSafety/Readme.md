
# Food Spoilage and Preserved Goods

Introduces food spoilage to the game, and new preserved foods that do not spoil.

## Features

* Disable all Screen Effects in the game. This means all of them. Such as the Drunk Effect, but also the radiation, paint effect, hot, cold, etc.

## Dependent and Compatible Modlets

**This modlet requires the [Gears](https://www.nexusmods.com/7daystodie/mods/4017) modlet or it will silently fail to do anything.**


## Technical Details

This modlet uses XPath to modify XML files, and does not require C#.

However, the [Gears](https://github.com/s7092910/Gears) modlet **does** require C# code.
It is *not* compatible with EAC.

It must be installed on both clients and servers.

After installation, **you absolutely must start a new game!**

If you load up an existing game after installing this modlet,
**it will become corrupted and you will lose the game world.**

### How Visual Safety works

This modlet depends upon the c# code provided by the [Gears](https://github.com/s7092910/Gears) modlet.
That modlet has custom C# code that is configurable via XML. Which has been leveraged to allow you to enable and disable the screen effects of the game from the main menu.

#### Feature configuration via Mods Menu

Select Mods from the Main Menu, then scroll through the list of mods until you find mjVisual Safety, which should be the last in the list, and select Yes to disable or no to enable all Screen Effects.

### Roadmap

I am working on adding in targeted Screen Effects settings.
Then Colorblind Selections as well to allow you to easily swap the colors used in the UI in the game to something more conducive to different forms of color blindness.
