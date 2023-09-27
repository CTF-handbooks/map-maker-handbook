# The Map Maker's Handbook

This is a guide on how to setup your game and world for map making. (Blocks are referred to as "nodes" in Minetest).

***
### 1. Required tools
* Minetest version 5.6 or above.
    > If you don't have Minetest installed, you can download it from the [official Minetest website](https://www.minetest.net/).
* Capture the Flag game for Minetest.
    > You can install the game from either the Minetest in-game ContentDB or from the [ContentDB website](https://content.minetest.net/packages/rubenwardy/capturetheflag/).
    
    > Once you downloaded the .zip file from the ContentDB website, extract the .zip file and move the folder inside it to `[Minetest folder]/games`.
* WorldEdit mod for Minetest (_optional_).
    > Although this is optional, it is recommended that you install WorldEdit. Creating maps requires you to build the borders and barriers of the map manually. This tool speeds the process up. This is also helpful when building other desired map structures.

    > You can install WorldEdit from either the Minetest in-game ContentDB or from the [ContentDB website](https://content.minetest.net/packages/sfan5/worldedit/).

    > Once you downloaded the .zip file from the ContentDB website, extract the .zip file and move the folder inside it to `[Minetest folder]/mods`.
  
***
### 2. Planning the map
* A map shouldn't be too big or too small. The size of a map can vary depending on the terrain and structures that the map will have. A maximum of `230 x 230` blocks in surface area is recommended.
* If you are making a map for the official CTF server, it is important to note that your map should be unique and not similar to the maps that already exist in the game.

    > "The design of a map should encourage differing gameplay and tactics." - -sniper-
* The design of a map shouldn't give any team advantages (such as having a better position or more resources). All teams should have an equal chance of winning.
* Using certain mods on the world the map-making takes place might cause unpredicted problems to the finished map. Switching Minetest or CTF game versions in the midst of the map-making process might also cause problems.
  
***
### 3. Creating the world
* Open Minetest and select the `Capture the Flag` game.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/d64da4d8-10e7-4a0e-b555-775f3804097b)
* Create a new world. You can use any mapgen. If you would like to use generated terrain, you can choose the `v7` or `flat` mapgen. If you plan on building the terrain/structures yourself, you can choose the `singlenode` mapgen. 

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/d49ea3a7-87b4-4d42-af98-e003790b8ad4)
* After you click `Create`, uncheck `Enable Damage` and check `Creative Mode`. Creative mode will enable `mapedit` mode.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/158625b3-5596-4143-8a7e-8969835c17a2)
* If you would like to use WorldEdit, click `Select Mods`, select `WorldEdit`, and click `Enable modpack`.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/a40dea59-fdab-459f-b2f8-5c281c037498)
* Click `Save` and play the world.
  
***
### 4. Setting up
* Grant yourself the "ctf_map_editor" by running `/grantme ctf_map_editor`. You can also use `/grantme all` to grant you "ctf_map_editor" and all the other privs that will be useful while making a map, such as fly, noclip, fast, etc...
* You can hit Esc on your keyboard and click `Change Keys` to see your controls (such as how to fly, noclip, etc...).

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/98117763-d42c-4a64-ade6-a894c14f61a9)
* *Tip*: run `/time 12000` and `/set -n time_speed 0` if you want to disable nighttime while building the map.

***
### 5. WorldEdit basics
* To use WorldEdit, first you must select an area in which your actions take place.
* You can use the `WorldEdit Wand tool` to select your area. To select your area, you select the two opposite corners of the area. Left-click a node with the tool to make the node the first corner, and right-click to set the second.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/fbf6847c-34ed-4c6b-892e-2c862aa3927f)
* An alternative method is to stand at the point you would like to select and run `//1` in chat to set the first corner, and `//2` to set the second.
* The area within will be selected.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/ee5175f2-5071-405f-a7f1-d175261002a9)
* **Remember to backup your world before risky operations!**
* Open your inventory. Under the `Crafting` tab you can see an earth icon hiden behind the crafting options. Click it to open the WorldEdit GUI

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/d8db8d4c-ee38-4d12-a90b-d2fb73884611)
* These are the tools that you can use to alter the nodes within your selected area. You can experiment with the options.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/ef0db7f5-696a-4611-ad54-c4def6d1aa2f)
* To set the area you've selected earlier with a certain type of node, click `Set Nodes`, type in the name of the node you would like to set in the field, click `search` or press enter, and click `Set Nodes`.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/3b12e708-f60e-42c4-8ebc-1a1c764dd093)

* If you've selected a large area, WorldEdit might give you a warning in chat. Type `//yes` in chat to continue.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/1e84188f-52a6-43db-a79c-fc662e75d987)
* To replace a certain type of node with another one in your selected area, select `Replace Nodes`. In the first field, type in the node you would like to replace, and in the second field, type in the node you would like to replace with.
* To only place nodes where there are no nodes, you can replace `air` with the node you want to use.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/63fe78c0-ab9f-458d-b6bd-7d90ea4414c5)

***
It is your choice to build the barriers first or the map first. For this example we are going to build the barriers first.
### 6. Removing the surrounding terrain
This is optional and only applies if you're using generated terrain.
* This is optional, but with generated terrain, it might be hard to place the outer barriers when the terrain outside your map area is blocking your view. An easy and recommended solution is to export the part of terrain you want to use and import it again into a singlenode world.
* Using WorldEdit, select or
### 8. Building the map
* Find a place to build your map and start building it. You can add any structure you want. Many blocks have indestructible variants, which you can use for builds you don't want players to destroy (use the admin pickaxe to break indestructible blocks).

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/3a724fe8-9005-4dde-9438-36d424a2e7be)
  
* You should also add the following:
    * Indestructible blocks under the position of the flag (the flag will be added later). The minimum surface area for this indestructible platform is `5x5` blocks (the flag should be in the middle).
    * Team chests for each team. You can find them as a node in the inventory.
      
      ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/74f210ba-3b94-473a-bff8-886f8578d3d3)
    * _Optional_: ores (such as iron, diamond, or mese ores). The amount of ores for each team should be about the same to ensure that no team has an advantage (please note that mapgens such as v7 and flat come with ores).
