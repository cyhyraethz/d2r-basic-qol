## Diablo II Resurrected Basic QoL

This is a basic quality of life mod for Diablo II Resurrected

### Features

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
  - Show item level

### Installation

1. Download the most recent release of basic-qol.mpq from the
   [releases page](https://github.com/cyhyraethz/d2r-basic-qol/releases)

2. Open your file manager and navigate to your Diablo II Resurrected installation directory,
   usually located in `C:\Program Files (x86)\Diablo II Resurrected`

3. Create a new folder named `mods` in the Diablo II Resurrected installation directory

4. Create a new folder named `basic-qol` in the new `mods` folder

5. Copy basic-qol.mpq into the new `basic-qol` folder, which should look like this:

   `C:\Program FIles (x86)\Diablo II Resurrected\mods\basic-qol\basic-qol.mpq`

6. Create a new shortcut for D2R.exe on your Desktop

7. Right click on the new shortcut, select properties, and add the `-mod basic-qol` parameters

8. Start Diablo II Resurrected using the new shortcut and enjoy the quality of life features

### How to Disable Features

I added safe unsocket and free respec as new cube recipes rather than modifying existing cube recipes so
that the old recipes would still be available. That way if you don't want those features you can simply
choose not to use those recipes and use the old ones instead (e.g. using a Hel rune to unsocket items,
destroying the removed gems/runes/jewels, and combining essences to create a Token of Absolution).

However, if you don't want those features and you feel uncomfortable even having them available in the
game, or if there are other features that you don't want, here are the steps for disabling features:

1. Download [MPQ Editor](http://www.zezula.net/en/mpq/download.html)

2. Start MPQ Editor and open basic-qol.mpq

3. Navigate to data/global/excel (you should see several .bin and .txt files on the right side)

4. Delete the .bin files that correspond to the feature you want to disable

You can also delete the corresponding .txt file if you want; it makes no difference.

Here are the files that are responsible for each feature:

- Stack Size
  - misc.bin
- Town Cast
  - skills.bin
  - missiles.bin
- Quest Bug
  - treasureclassex.bin
- Unsocket
  - cubemain.bin
- Respec
  - cubemain.bin
- Item Level
  - armor.bin
  - misc.bin
  - weapons.bin

Note: deleting .bin files will disable all features for which they are responsible.

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

Item Storage:

- [Collection Manager](https://youdz.github.io/d2-stash-organizer/) - item storage and management

Holy Grail:

- [Grail Tracker](https://d2-holy-grail.herokuapp.com/) - website for tracking grail progress

Community:

- [r/diablo2](https://www.reddit.com/r/diablo2/) - helpful and active reddit community
