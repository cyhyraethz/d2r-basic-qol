## Diablo II Resurrected Basic QoL

This is a basic quality of life mod for Diablo II Resurrected

### Main Features

- Stack Size
  - Key stack size increased from 12 to 50
  - Tome stack size increased from 20 to 80
  - Arrow and bolt stack size increased to 500
- Town Cast
  - Enable additional spells to be cast in town
    - Teleport, Thunderstorm, Armageddon, Hurricane
    - Charge, Leap, Shout, Battle Orders, Battle Command
  - Allow some spells to be cast in Werewolf and Werebear
    - Teleport, Shout, Battle Orders, Battle Command
- Quest Bug
  - Always get quest drops from Andariel
  - Even if you forget to talk to Warriv
- Unsocket
  - New cube recipe for unsocketing
  - Scroll of Town Portal + Socketed Item
  - Unsockets items without destroying runes
- Respec
  - Free, unlimited respeccing
  - New cube recipe for respec token
  - Scroll of Town Portal + Scroll of Identify
- Item Level
  - Display item level next to item names
- World Event
  - Herbs can be bought from Gheed
  - Herbs can be sold to spawn Diablo Clone
  - Standard of Heroes can also spawn Diablo Clone

### Optional Features

- Loot Filter
  - Highlights important items
  - Shortens the names of junk drops
- Expanded Storage
  - Inventory increased to 8x10
  - Stash and cube increased to 13x16

### Installation

1. Download the most recent release from the
   [releases page](https://github.com/cyhyraethz/d2r-basic-qol/releases)
   and extract the files

2. Transfer offline save files into the basic-qol save folder
   ([link to instructions](#how-to-transfer-save-files))

3. Add any optional features that you want to include
   ([link to instructions](#how-to-add-optional-features))

4. Open your file manager and navigate to your D2R installation directory,
   usually located in `C:\Program Files (x86)\Diablo II Resurrected`

5. Create a folder named `mods` in the D2R installation directory if it doesn't already exist

6. Create a folder named `basic-qol` in the `mods` folder if it doesn't already exist

7. Copy `basic-qol.mpq` into the `basic-qol` folder, which should look like this:

   `C:\Program FIles (x86)\Diablo II Resurrected\mods\basic-qol\basic-qol.mpq`

8. Create a new shortcut for D2R.exe on your Desktop

9. Right click on the new shortcut, select properties, and add the `-mod basic-qol -txt` parameters

10. Start Diablo II Resurrected using the new shortcut and enjoy the quality of life features

### How to Transfer Save Files

1. Open your file manager and navigate to your D2R save file directory,
   usually located in `C:\Users\Username\Saved Games\D2R`

2. Create a folder named `mods` in the D2R save file directory if it doesn't already exist

3. Create a folder named `basic-qol` in the `mods` folder if it doesn't already exist

4. Copy and paste your character save files into the `basic-qol` folder

### How to Add Features

You may be able to combine other mods using this method as well, as long as they don't rely on any of the
same modded files (e.g. misc.txt). If you're not sure if they do or not but want to try anyway, I recommend
backing up your basic-qol.mpq before attempting to merge the data folders. If it asks you whether it should
replace a file then there is a conflict. Restore from your backup and consider the mods incompatible.

1. Open the `basic-qol.mpq` and `optional` folders in your file manager (e.g. Windows Explorer)

2. Navigate to the optional subdirectory for the feature that you want to add (e.g. lootfilter)

3. Copy the `data` folder into `basic-qol.mpq` and select merge when prompted

### How to Disable Features

I added safe unsocket and free respec as new cube recipes rather than modifying existing cube recipes so
that the old recipes would still be available. That way if you don't want those features you can simply
choose not to use those recipes and use the old ones instead (e.g. using a Hel rune to unsocket items,
destroying the removed gems/runes/jewels, and combining essences to create a Token of Absolution).

However, if you don't want those features and you feel uncomfortable even having them available in the
game, or if there are other features that you don't want, here are the steps for disabling features:

1. Open `basic-qol.mpq` in your file manager (e.g. Windows Explorer)

2. Navigate to `data/global/excel` (you should see several .txt files in this directory)

3. Delete the .txt files that correspond to the feature you want to disable

Here are the files that are responsible for each feature:

- Stack Size
  - misc.txt
- Town Cast
  - skills.txt
  - missiles.txt
- Quest Bug
  - treasureclassex.txt
- Unsocket
  - cubemain.txt
- Respec
  - cubemain.txt
- Item Level
  - armor.txt
  - misc.txt
  - weapons.txt
- World Event
  - misc.txt

Note: deleting .txt files will disable all features for which they are responsible.

### Additional Notes

If your cursor is on top of an NPC when casting Teleport in town it will register as you clicking on them
and your character will move toward them normally. You can get around this by holding down the Show Items
hotkey to prevent your character from targeting the NPC, allowing you to Teleport right next to them.

Hurricane and Armageddon can be precast in town but will not display their animations until you leave town.

### Resources

Drop Calculator:

- [Silospen Drop Calculator](https://dropcalc.silospen.com/item.php?np=1&ng=1&mf=0&dec=false&mk=&diff=&qual=&ver=-1&version=113) - website for calculating drop rates

General Information:

- [The Arreat Summit](http://classic.battle.net/diablo2exp/) - original source of game information
- [Diablo 2 Wiki](https://diablo2.diablowiki.net/Main_Page) - wiki pages for every aspect of the game
- [Cheat Sheet](https://htmlpreview.github.io/?https://github.com/Michaelangel007/d2_cheat_sheet/blob/master/index.html) - dense resource with tons of information

Item Storage:

- [Collection Manager](https://youdz.github.io/d2-stash-organizer/) - item storage and management

Holy Grail:

- [Grail Tracker](https://d2-holy-grail.herokuapp.com/) - website for tracking grail progress

Community:

- [r/diablo2](https://www.reddit.com/r/diablo2/) - helpful and active reddit community

Map Tool:

- [D2MapTools](https://gitgud.io/stephenlynx/D2MapTools) - script for saving map seeds

### Credits

Loot filter created by Cbraqz

Expanded storage created by Bonesy
