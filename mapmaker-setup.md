# The Map Maker's Handbook

This is a guide on how to setup your game and world for map making.

### 1. Required Tools
* Minetest version 5.6 or above.
    > If you don't have Minetest installed, you can download it from the [official Minetest website](https://www.minetest.net/).
* Capture the Flag game for Minetest.
    > You can install the game from either the Minetest in-game ContentDB or from the [ContentDB website](https://content.minetest.net/packages/rubenwardy/capturetheflag/).
    
    > Once you downloaded the .zip file from the ContentDB website, extract the .zip file and move the folder inside it to `[Minetest folder]/games`.
* WorldEdit mod for Minetest (_optional_).
    > Although this is optional, it is recommended that you install WorldEdit. Creating maps requires you to build the borders and barriers of the map manually. This tool speeds the process up. This is also helpful when building other desired map structures.

    > You can install WorldEdit from either the Minetest in-game ContentDB or from the [ContentDB website](https://content.minetest.net/packages/sfan5/worldedit/).

    > Once you downloaded the .zip file from the ContentDB website, extract the .zip file and move the folder inside it to `[Minetest folder]/mods`.

### 2. Planning the map
* A map shouldn't be too big or too small. The size of a map can vary depending on the terrain and structures that the map will have. A maximum of `230 x 230` blocks in surface area is recommended.
* If you are making a map for the official CTF server, it is important to note that your map should be unique and not similar to the maps that already exist in the game.

    > "The design of a map should encourage differing gameplay and tactics." - -sniper-
* The design of a map shouldn't give any team advantages (such as having a better position or more resources). All teams should have an equal chance of winning.
* Using certain mods on the world the map-making takes place might cause unpredicted problems to the finished map. Switching Minetest or CTF game versions in the midst of the map-making process might also cause problems.

### 3. Creating the World
* Open Minetest and select the `Capture the Flag` game.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/d64da4d8-10e7-4a0e-b555-775f3804097b)
* Create a new world. You can use any mapgen. If you would like to use generated terrain, you can choose the `v7` or `flat` mapgen. If you plan on building the terrain/structures yourself, you can choose the `singlenode` mapgen. 

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/d49ea3a7-87b4-4d42-af98-e003790b8ad4)
* After you click `Create`, uncheck `Enable Damage` and check `Creative Mode`. Creative mode will enable `mapedit` mode.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/158625b3-5596-4143-8a7e-8969835c17a2)
* If you would like to use WorldEdit, click `Select Mods`, select `WorldEdit`, and click `Enable modpack`.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/a40dea59-fdab-459f-b2f8-5c281c037498)
* Click `Save` and play the world.

### 4. Setting Up
* Grant yourself the "ctf_map_editor" by running `/grantme ctf_map_editor`. You can also use `/grantme all` to grant you "ctf_map_editor" and all the other privs that will be useful while making a map, such as fly, noclip, fast, etc...
* You can hit Esc on your keyboard and click `Change Keys` to see your controls (such as how to fly, noclip, etc...).

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/98117763-d42c-4a64-ade6-a894c14f61a9)
* *Tip*: run `/time 12000` and `/set -n time_speed 0` if you want to disable nighttime while building the map.
