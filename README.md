# ValheimPlus
A HarmonyX Mod aimed at improving the gameplay quality of Valheim



# Configuration File

The Config files name is supposed to be "valheim_multipliers.cfg" it needs to be placed in "BepInEx\config"
(The name will be adjusted in the future)
You will also need to place the "INIFileParser.dll" into the "BepInEx\plugins" folder (its supplied by default within the release versions)

# Currently Supported Configuration
```INI
[Player]
baseMegingjordBuff=200
; default is 150 (float)
; Ingame Tooltip is not affected

baseMaximumWeight=300
; default is 300 (float)

baseAutoPickUpRange=2
; default is 2 (float)


[Food]
foodDurationMultiplier=5.0
; default is 0, it adds to the value meaning 0.0 is 100%, 1 is 200%.

[Fermenter]
fermenterDuration=2400
; default is 2400 (float) (24 ingame hours ?)

fermenterItemsProduced=4
; default is 4 (integer) items per fermenter process

[Furnace]
maximumOre=20
;default is 10 (int)

maximumCoal=20
;default is 10 (int)

productionSpeed=2
;default it 10 (float)

coalUsedPerProduct=1
;default is 4 (int)

[Items]
noTeleportPrevention=true
;default is false (boolean)

baseItemWeightReduction=0
;(float), removes from value (original - (original * baseItemWeightReduction). 
;1 is 100% weight reduction of every item, 0.5 is 50%.

[Building]
noInvalidPlacementRestriction=true
;(boolean)

[Beehive]
enabled=true

maximumHoneyPerBeehive=7
;(integer)

honeyProductionSpeed=1
;(float), default is 10. Do not go lower than 5.
```
# Valheim Plus Compiler Requirements

You will be dependent on a package of stripped .net/mono Unity files from the Valheim directory.
How to get BepInEx working:

1. Download this package:

https://mega.nz/file/0UAlxQwK#47InGOb8ViI6GyBDArpbhkbMTBklXdyRSmAc4-BZpJY

2. Unpack into your Valheim root folder and overwrite every file when asked.

3. Add all dll's of "\Valheim\valheim_Data\Managed" folder as references to the project.

(Except : "mscorlib.dll", "System.Configuration.dll", "System.Core.dll", "System.dll", "System.Xml.dll")

4. Add all BepInEx dll's ("Valheim\BepInEx\core") as refernces to the project.

(Except : "0Harmony.dll", "0Harmony20.dll")

5. Add Ini-parser and HarmonyX via nu-get

# Credits

nx#8830 - All (as of now)
