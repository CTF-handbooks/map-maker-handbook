# The Map Maker's Handbook

This is a detailed guide on how to create a map for the Minetest Capture the Flag game.

### 1. Required Tools
* Minetest version 5.6 or above.
    > If you don't have Minetest installed, you can download it from the [official Minetest website](https://www.minetest.net/).
* Capture the Flag game for Minetest.
    > You can install the game from either the Minetest in-game ContentDB or from the [ContentDB website](https://content.minetest.net/packages/rubenwardy/capturetheflag/).
    
    > Once you downloaded the .zip file from the ContentDB website, extract the .zip file and move the folder inside it to `[Minetest folder]/games`.
* WorldEdit mod for Minetest (_optional_).
    > Although this is optional, it is recommended that you install WorldEdit. Creating maps requires you to build the borders and barriers of the map manually. This tool speeds the process up. This is also helpful when building other map structures.

    > You can install WorldEdit from either the Minetest in-game ContentDB or from the [ContentDB website](https://content.minetest.net/packages/sfan5/worldedit/).

    > Once you downloaded the .zip file from the ContentDB website, extract the .zip file and move the folder inside it to `[Minetest folder]/mods`.

### 2. Planning the map
* A map shouldn't be too big or too small. The size of a map can vary depending on the terrain and structures that the map will have. A maximum of *230 x 230* blocks in surface area is recommended.
* If you are making a map for the official CTF server, it is important to note that your map should be unique and not similar to the maps that already exist in the game.

    > "The design of a map should encourage differing gameplay and tactics." - -sniper-
* The design of a map shouldn't give any team advantages (such as having a better position or more resources). All teams should have an equal chance of winning.
* Using certain mods on the world the map-making takes place might cause unpredicted problems to the finished map. Switching Minetest or CTF game versions in the midst of the map-making process might also cause problems.

### 3. Creating the World
* Open Minetest and select the Capture the Flag game.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/8fc4f325-b209-4f38-9044-a42fae90a5e2)
* Create a new world. You can use any mapgen. You can use the v7 mapgen for generated terrain, or you can use the flat or singlenode mapgen if you want to make a map from scratch.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/0fbc627f-2edd-45c4-a740-754f2b51e99b)
* After you click `Create`, uncheck `Enable Damage` and check `Creative Mode`. Creative mode will enable `mapedit` mode.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/a0f79ad7-689b-46cb-8f6a-c50a0436b7de)
* If you would like to use WorldEdit, click `Select Mods`, select `Minetest-WorldEdit`, and click `Enable modpack`.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/c9222045-52c1-4945-9377-bde3cd345088) ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/5c29118f-409c-4e97-8283-01d7be6ec976)
* Click `Save` and play the world.

### 4. Setting Up
* Grant yourself the "ctf_map_editor" by running `/grantme ctf_map_editor`. You can also use `/grantme all` to grant you "ctf_map_editor" and all the other privs that will be useful while making a map, such as fly, noclip, fast, etc...
* You can hit Esc on your keyboard and click `Change Keys` to see your controls (such as how to fly, noclip, etc...).

### 5. Building the Map
* It is your choice to build the borders or map first. For this example, we will build the map first.

  > If you are using a singlenode mapgen, you can't move without noclip enabled. You'll need to replace the area you would like to build your map in with `air` using WorldEdit (a link to the WorldEdit handbook will be down below).
* Find a place to build your map and start building it. You can add any structure you want. Many blocks have indestructible variants, which you can use for builds you don't want players to destroy (use the admin pickaxe to break indestructible blocks).

  > To build better builds on your map, you can check out this handbook: <WIP, will add later>.
  
  > *Tip*: run `/time 12000` and `/set -n time_speed 0` if you want to disable nighttime while building the map.
* You should also add the following:
    * Indestructible blocks under the position of the flag (the flag will be added later). The minimum surface area for this indestructible platform is `5x5` blocks (the flag should be in the middle).
    * Team chests for each team. You can find them as a node in the inventory.
      
      ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/74f210ba-3b94-473a-bff8-886f8578d3d3)
    * _Optional_: ores (such as iron, diamond, or mese ores). The amount of ores for each team should be about the same to ensure that no team has an advantage (please note that mapgens such as v7 and flat come with ores).

### 6. Building the Barriers
* The barriers should prevent the players from escaping the map. The barriers can be any indestructible block. "Indestructible Barrier Glass" (`ctf_map:ind_glass`) around the edge and "Indestructible Stone" (`ctf_map:stone`) for the bottom of the map is typical.
* You can leave the roof open. Players shouldn't be able to escape if you set your map area correctly.
* It is your choice to put the barriers at the edge of the map or leave parts of your map outside the barrier.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/97c838aa-1fea-4d4e-bd23-d49d563de4a6) ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/29591651-35a6-48b2-8095-1c5dde26c2b7)
* The build-time wall should be placed in the middle of the map. Use "Indestructible Red Barrier Glass" (`ctf_map:ind_glass_red`) for the parts of the wall that consists of air (no blocks) and "Indestructible Red Barrier Stone" (`ctf_map:ind_stone_red`) for the parts of the wall that consists of stone blocks. You can choose to not add the red barrier stones depending on the design of the map. The red barrier glass will disappear and the red barrier stone will turn into normal stone once the match starts.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/d06602c8-1f60-416e-86af-430448ea26a2)
* On how to use WorldEdit, you can check out this tutorial: (the WorldEdit handbook is still a WIP, for now, this tutorial will do: https://youtu.be/7qQ6w0ntk9g?t=110)
