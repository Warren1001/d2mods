# In-game Hero Editor for D2R

## Last updated for D2R 3.3 (93847)

If you find a bug or crash or any problem related to this mod, please report it to me through the Issues tab.  

The purpose of this mod is to have an in-game testing tool that is significantly more convenient for basic item generation than an external hero editor. It remains as close to unmodded as possible, modifying nothing existing, and only adding new mechanics. With that said, some things have to be altered to make features of this mod possible:
- Horadric Cube name will appear like a normal item.
- Horadric Cube will likely no longer trigger quest statuses, but quests should still complete normally.
- Item buy values have been reduced significantly and item sell values have been increased significantly.
- Sell value cap raised significantly.
- Unique item rarities have been flattened, making all unique items the same rarity (ie Templar's Might and Tyrael's might have a 50/50 chance instead of a 7/1 ratio).
- Renewed Sunder charms can drop from monsters (byproduct of enabling them for Cube Recipes).
- All monsters can drop any Sunder charm (as long as they are sufficiently high enough level).
- Unique items can spawn an unlimited amount of times in one game.
- Gambling screen has all item bases.
- Some items that aren't typically droppable via monsters may now be able to (unintentionally).
- All movement skills are enabled in town.
- Teleporting through walls is allowed in Duriel's Chamber.
- You can carry as many unique charms as you want without restriction.

It is important to note that items found naturally while playing with this mod will still contribute to your Chronicle. You won't get banned if you accidentally log into online with the mod, but several things won't work correctly and give you errors, such as vendoring.

I tried my best to establish a pattern for cube recipes.  
Here are the relevant changes of the mod:  
- Akara's Misc page has a ton of items for sale, many of which are used for cube recipes also added by the mod.
- Added a bunch of cube recipes. All original cube recipes are untouched.

Everything this mod allows you to do should be compatible with Vanilla. The Horadric Cube isn't marked as a quest item in the technical sense so it may look weird in-game, but Vanilla and hero editors should be fine with it.

## How to Install

If you run into problems installing, you can make an issue here on GitHub, send me a message on Discord (Warren1001), or email me at kabryxis@gmail.com.  
If you have problems installing or using D2RLoader and I'm not immediately available, go to their Discord and post in their support channel and they'll be happy to help.  

When updating this mod to a new version, **do not** drag and drop the mod files and replace the old ones. Delete the old mod folder entirely before installing a new version. Simply replacing files does not always work for updating D2 mods.  

### D2RLoader

I highly recommend using the D2RLoader version of the mod, as D2RLoader has many developer debug features available, allowing a lot of cheat functionality for controlling your character's data, generating items, and so much more.

1. Install [D2RLoader](https://d2rloader.net). Their website has installation instructions.
2. Download the latest `d2rloader-ighe.zip` file from the [Releases]() page.
3. Navigate to your D2R install.
4. Navigate to the mods folder. If you do not have one, just create one. Your path should be `{D2R base folder}\mods`.
5. Extract the `ighe` folder from the ZIP file into the mods folder. If you've done it correctly, you should see a path similar to `{D2R base folder}\mods\ighe\ighe.mpq\...`.
6. Launch D2RLoader using D2RLoader.exe in your D2R folder.
7. Open the D2RLoader settings from the main menu (gear icon below `Play` button) and change `Default Mod` to `ighe`, then restart as it asks.
8. Done. Load into a game and begin playing.

### Vanilla

If you really don't want to use D2RLoader, which I highly recommend to use, then:

1. Download the latest `vanilla-ighe.zip` file from the [Releases]() page.
2. Navigate to your D2R install.
3. Navigate to the mods folder. If you do not have one, just create one. Your path should be `{D2R base folder}\mods`.
4. Extract the `ighe` folder from the ZIP file into the mods folder. If you've done it correctly, you should see a path similar to `{D2R base folder}\mods\ighe\ighe.mpq\...`.
5. Go to Battle.net and click the Gear Icon next to Play for D2R, then click Game Settings.
6. Tick the box that is labeled `Additional command line arguments`.
7. Paste the following into the text box that shows up: `-mod ighe -txt -enablerespec`. The `-enablerespec` option grants free respecs by Alt + Left Clicking on the stat point allocation buttons in the character screen (only if you've allocated points to that stat).
8. Done. Launch the game and load into a game and begin playing.

## How to Get a Character Started

### D2RLoader

The initial process can be sped up with a hero editor such as [d2emu's hero editor](https://d2emu.com/hero), but D2RLoader makes the process quick and easy as well.

Ensure Developer Console is enabled in the D2RLoader settings in the main menu. You can open and close the Developer Console with Ctrl+` (above Tab, next to 1).
1. Create a character and head in-game.
2. Open the Developer Console.
3. Type the command `debug mode`.

You can now use all of the developer features. Explore around, I will not be explaining them all here. The [D2RLoader website](https://d2rloader.net) and their Discord (found on their website) can offer more support and information for the developer debug features. Many of these features will be easier to use than the functionality provided by this mod to gain access to various items once you've learned how to use them. The two main things you will be interested in is the `Debug Tools` button at the top left and the cheat commands, which you can see by typing the command `help cheats` into the Developer Console.

1. Type the command `cheat level 99` (or whatever level you'd like your character to be).
2. Type the command `cheat waypoints` to unlock all waypoints in the current difficulty.
3. Type the command `cheat quests` to complete all quests in the current difficulty.
4. Repeat 2 and 3 for each difficulty.

Remember to enable `Save Cheat Items` under `Debug Tools > Cheat Status` if you use D2RLoader functionality to spawn items and want the items to persist between games!

### Vanilla

Your best bet is using an existing character or generating one with a Hero Editor. [d2emu has a great Hero Editor](https://d2emu.com/hero).

## New Cube Recipes

For anything that is numerical, counting is done with runes. El Rune is 1. Eld Rune is 2. etc

To add a socket to an unsocketed item, use the numerical equivalent rune for the number of sockets you want on the item. If the recipe doesn't work, that item can't have that many sockets. Check the item level if you think it should. Items that are already socketed cannot have their socket count modified.
- Item + El Rune = Item with 1 Socket
- Item + Eld Rune = Item with 2 Sockets
- ...etc

In the event you have an item whose item level is too low for sockets or a specific rarity:
- Item + Hel Rune = Item with `item level = 99`

If you want to remove the sockets of an item without destroying them:
- Socketed Item + Hel Rune + Scroll of Identify = Open Socketed Item + Socket Items

To change the rarity of an item, use the associated perfect gem color. Since there isn't a gold gem (Unique) and Normal and Superior items are both white:
- Item + Perfect Skull = Item with Normal Quality
- Item + Perfect Diamond = Item with Superior Quality
- Item + Perfect Sapphire = Item with Magic Quality
- ...etc
- Item + Perfect Amethyst = Item with Unique Quality

If you change an item quality to the same item quality it already has, this will effectively reroll the item.

To change the tier of an item, use a Perfect Ruby.
- Normal Item + Perfect Ruby = Exceptional Item
- Exceptional Item + Perfect Ruby = Elite Item

There is no way to downgrade, D2R doesn't seem to support this. If you need to go down a tier, you'll have to acquire that manually (I use Gambling).

To make an item ethereal:
- Item + Zod Rune = Ethereal Item

Cubing a Tome of Town Portal by itself will open the Cow Portal for convenience. The original recipe still exists.

### To acquire skiller Grand Charms:

The numerical order is based on the order of the skill tabs on the skill tree in-game. For example, Cold Spells is the first skill tab on the skill tree in-game for the Sorceress, so Cold Spells = 1. Lightning Spells = 2. etc
- Magic Grand Charm + numerical rune of the skill tree tab order = New Magic Grand Charm with Tab Skill.

Examples:
- As a Sorceress: Magic Grand Charm + El Rune = New Magic Grand Charm with +1 to Cold Skills
- As an Amazon: Magic Grand Charm + El Rune = New Magic Grand Charm with +1 to Javelin and Spear Skills
- As a Warlock: Magic Grand Charm + Tir Rune = New Magic Grand Charm with +1 to Demon Skills

### Sunder Charms

New convenience recipes were added that are the same as original recipes but without the shards.  
The materials will be refunded allowing you to craft again.  
A Renewed Sunder charm can only be obtained by crafting a Latent Sunder charm into a Renewed Sunder charm.  
A Renewed Sunder charm can be used to craft itself again using the same ingredients as the Latent recipe.  
Additionally, once you have a Renewed Sunder charm, you can also use the Unique recipe (Perfect Amethyst) to reroll into any Renewed Sunder charm.  

### Colossal Jewels

Akara sells two jewels. The one closest to the runes is the normal jewel. The other one is the colossal jewel base. You can craft Colossal Jewels using the Unique recipe (Perfect Amethyst) with the colossal jewel base.  

### D2RLoader

If you are using D2RLoader, you can clone any item exactly by placing it in the Horadric Cube by itself and transmuting. If the item is two slots wide, the cloned item will appear slightly outside of the Horadric Cube, but this is to be expected.  

### Other

For Crafted items, the recipe is the same however you only need the rune and a Scroll of Identify. The gem and the jewel are no longer needed. The recipe will return the rune and scroll for you to craft again.  
Additionally, you can use crafted items to re-roll the craft, so you don't need to keep getting magic items.  
Lastly, the item level of the crafted item is always the item level of the original item. The item level will never change. Character level no longer matters.  
The original crafting recipes still exist.  

There is no way to acquire specific Rare items or any other Magic items besides blindly rerolling, using D2RLoader's developer debug features, or using a hero editor.  
