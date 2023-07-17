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
* A map shouldn't be too big or too small. The size of a map can vary depending on the terrain and structures that the map will have. A maximum of *230 x 230x* blocks in surface area is recommended.
* If you are making a map for the official CTF server, it is important to note that your map should be unique and not similar to the maps that already exist in the game.

    > "The design of a map should encourage differing gameplay and tactics." - -sniper-
* Using certain mods on the world the map-making takes place might cause unpredicted problems to the finished map. Switching Minetest or CTF game versions in the midst of the map-making process might also cause problems.

### 3. Creating the World
* Open Minetest and select the Capture the Flag game.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/5cce3993-a5f4-408a-9178-c177f5e6885a)
* Create a new world. You can use any mapgen. You can use the v7 mapgen for generated terrain, or you can use the flat or singlenode mapgen if you want to make a map from scratch.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/0fbc627f-2edd-45c4-a740-754f2b51e99b)
* After you click `Create`, uncheck `Enable Damage` and check `Creative Mode`. Creative mode will enable `mapedit` mode.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/a0f79ad7-689b-46cb-8f6a-c50a0436b7de)
* If you would like to use WorldEdit, click `Select Mods`, select `Minetest-WorldEdit`, and click `Enable modpack`.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/c9222045-52c1-4945-9377-bde3cd345088) ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/5c29118f-409c-4e97-8283-01d7be6ec976)
* Click `Save` and play the world.

### 4. Building the Map
* To get started, grant yourself the "ctf_map_editor" by running `/grantme ctf_map_editor`. You can also use `/grantme all` to grant you "ctf_map_editor" and all the other privs that will be useful while making a map, such as fly, noclip, fast, etc...
* You can hit Esc on your keyboard and click `Change Keys` to see your controls (such as how to fly, noclip, etc...).
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/c52147db-fe5c-48b9-932f-0f725df5c470)
