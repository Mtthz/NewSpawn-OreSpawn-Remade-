# Changelog

All NewSpawn updates, newest first. Downloads: [CurseForge](https://www.curseforge.com/minecraft/mc-mods/newspawn-oresspawn/files).

## v1.2.09 (21/11/2026)

### ✨ NEW

- Anvil repair: NewSpawn tools and armor can now be repaired at the anvil with the material they are made from, just like diamond tools with diamonds. Each material repairs 1/4 of the durability, and you can rename the item at the same time. Examples: ruby, amethyst, emerald, titanium or uranium ingot (Ultimate), Pink Tourmaline, Tiger's Eye, crystal planks and crystal stone, Mothra, Mobzilla, Queen and Nightmare scales, peacock feather, lava eel and lapis block.
- Rideable pets (Young Prince, Adult Prince, Leonopteryx, Dragon and Ostrich): Shift + right-click with an empty hand now makes them sit or stand up, like the Cephadrome. Right-clicking without Shift still mounts them.
- When you make a pet sit or stand up, a message shows above the hotbar: "<pet name>: sitting" or "<pet name>: free".

### 🛠️ FIXES

- Sitting pets now stay put. The Prince and The Princess no longer get up and fly after you when you walk more than 16 blocks away.
- Girlfriend, Boyfriend, Water Dragon, Camarasaurus and Ostrich no longer leave their spot while sitting (before, they still followed food, ran away, went indoors at night or walked to attack).
- Infinite Royal Guardian Sword: removed a stray white line that appeared next to the sword in first person. The other 3D Infinity items got the same fix.

## v1.2.08 (18/11/2026)

### 🛠️ FIXES

- Fixed a crash on game startup (ArrayIndexOutOfBoundsException in Biome.getSpawnableList) in big modpacks. It happened when another mod registers a new creature type too late during loading. Thanks to kasia1403 for the report!
- NewSpawn now safely skips creature types that Minecraft doesn't recognize, so the game loads normally.
- The same problem could also crash the world as soon as mobs started spawning. Now the natural spawning of those unrecognized creature types is turned off instead, so the world keeps running. All other mobs (vanilla, NewSpawn and other mods) spawn normally.
- When this happens, the log shows a warning with the name of the creature type, to help find which mod created it.

## v1.2.07 (07/11/2026)

### ✨ NEW

- Title screen: new "!" button next to Quit Game to report bugs. It opens the NewSpawn issues page on GitHub. It can be turned off with the reportButton option in the config.
- Girlfriend and Boyfriend are now drawn 1.6 blocks tall, matching their hitbox (the giant version is 8 blocks tall).

### 🔗 ADDONS WITH OTHER MODS

- HBM's NTM CE: Space: NewSpawn no longer crashes the game during startup when NTM:CE Space is installed. The planet biomes don't accept mob spawns, so NewSpawn mobs now skip them. Thanks to gdbiv for the report!

### 🛠️ FIXES

- Config: turning off the spawns.modBiomes option now also works for the mobs that spawn in "all biomes". With it off, they only spawn in vanilla Minecraft biomes.

## v1.2.06 (02/11/2026)

### ✨ NEW

- Title screen: a mini The Queen now flies after your mouse. Click her to switch between her normal and dark colors. While she's dark, clicking anywhere outside the buttons releases purple orbs that chase your mouse and fade after a few seconds. It can be turned off with the menuQueen option in the config.
- Title screen: the "Java Edition" banner now reads "NewSpawn Edition".

## v1.2.05 (02/11/2026)

### ✨ NEW

- Infinite Royal Guardian Armor (requires Avaritia): the Royal Guardian armor with animated cosmic lines. Crafted at the Extreme Crafting Table from the Royal Guardian piece and the matching Infinity piece.
- With the full set you still get hit, but take 0 damage. Each time a mob hits you, 10 of The Queen's purple orbs come out and chase it and nearby monsters. Each orb deals 50 damage and lasts up to 60 seconds.
- Each piece also has the power of the matching Infinity armor piece: Helmet - endless air, full hunger and night vision. Chest Plate - flight and removes bad effects. Leggings - you don't stay on fire. Boots - faster movement, higher jump, step up 1 block and no fall damage.
- Infinite Royal Guardian Sword and Armor: new item descriptions.
- Structure preview (Build button in /orespawn): your crosshair now targets the center of the structure, the mouse wheel rotates it to any of the 4 sides, and the Up and Down arrow keys move it up and down. The keys can be changed in Options > Controls.

### 🛠️ FIXES

- Avaritia: fixed a crash during game startup (pre-initialization) that could happen with Avaritia installed.
- Infinite Squid Zooka: the shot no longer kills its own squid.
- Squid Zooka: shot squids no longer drop items, which allowed an endless item farm.
- /orespawn: the Extreme Crafting Table recipe no longer appears black on items that also show a crafting table recipe.

## v1.2.03 (02/11/2026)

### 🛠️ FIXES

- Avaritia: fixed a crash during game startup (pre-initialization) that could happen with Avaritia installed.

## v1.2.02 (01/11/2026)

### 🛠️ FIXES

- Structure preview (Build button in /orespawn): your crosshair now targets the center of the structure instead of its corner.
- Structure preview: the mouse wheel now rotates the structure to any of the 4 sides, and the Up and Down arrow keys move it up and down. The structure is built exactly as previewed, including chests, spawners, doors and mobs. The keys can be changed in Options > Controls.

## v1.2.01 (01/11/2026)

### 🛠️ FIXES

- Language: chat and on-screen messages now follow the game's language. Before, they always appeared in Portuguese, even with the game in English. This covers messages from the Gamma Metroid, tamed pets, dragons, /orespawn, structure placement and dimension travel.
- /orespawn: 38 items were missing their English "How to use" text. All of them have it now.
- /orespawn: biome names now follow the game's language instead of always showing in Portuguese.
- Gamma Metroid: the title of its chest screen now follows the game's language.

## v1.2.00 (31/10/2026)

### ✨ NEW

- Additional Structures: 171 new structures (vanilla blocks only) in a new "Additionals" folder on the Structures tab of /orespawn. Each one has a button to choose whether it generates in the world, and the button shows where it generates: "Generates in world", "Generates in the Nether" or "Generates in The End". They all start disabled; this button works in survival too. "Build" (with a preview ghost) is creative only.
- Additional Structures: the bigger the structure, the rarer it is. The info page shows its chance, and very large ones show a warning that they can be heavy for the world.
- The End: Ender Castle, Ender Knight Dungeon and Cephadrome Altar now also generate in The End, on the outer islands and on the dragon island (away from the exit portal).
- /orespawn now recognizes other mods (view only): creatures, items, blocks and dimensions from Minecraft and other installed mods, each in its own folder. In creative you can spawn, take and teleport.
- /orespawn: folder colors to tell them apart: NewSpawn in yellow, Minecraft in light green, other mods in light red.

### 🔗 MOD COMPATIBILITY

- Avaritia: the item info page now shows the Extreme Crafting Table (9x9) and Compressor recipes.

### 🛠️ FIXES

- /orespawn: some creature names in the list were shown in a dark color; all names now use the normal color.
- /orespawn: removed the "Spawn" button from the Ender Dragon (it didn't work properly).

## v1.1.06 (30/10/2026)

### 🛠️ FIXES

- Shaders: in the mod's 6 dimensions, with shaders on, the world looked completely flat, with no shadows or lighting. The dimensions now use the same look as the Overworld with any shader pack. This can be turned off in the config (orespawnport_dimensoes.cfg, option shadersAsOverworld).

## v1.1.05 (30/10/2026)

### 🛠️ FIXES

- Shaders: with a caught ant, termite or butterfly on screen, the rest of the screen turned red or black, depending on the shader. The screen now looks normal.

## v1.1.04 (30/10/2026)

### 🛠️ FIXES

- /orespawn screen: the 3D preview of structures and creatures was small and stuck at the bottom, leaving a big empty space above it. It now starts right below the info and fills the space down to the bottom, so it's much bigger.
