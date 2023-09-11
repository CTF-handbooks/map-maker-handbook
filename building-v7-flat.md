# Building the Map and Barriers for `v7` or `flat`

It is your choice to build the barriers first or the map first. For this example we are going to build the barriers first.

### 1. WorldEdit basics
* To use WorldEdit, first you must select an area in which your actions take place.
* You can use the `WorldEdit Wand tool` to select your area. To select your area, you select the two opposite corners of the area. Left-click a node with the tool to make the node the first corner, and right-click to set the second.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/fbf6847c-34ed-4c6b-892e-2c862aa3927f)
* An alternative method is to stand at the point you would like to select and run `//1` in chat to set the first corner, and `//2` to set the second.
* The area within will be selected.

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/ee5175f2-5071-405f-a7f1-d175261002a9)
* **Remember to backup your world before risky operations!**

### 2. Exporting your area (optional and experimental)
With generated terrain, it might be hard to add the barriers with terrain blocking your view. This method can remove the extra terrain around your map.
> If you are building the barriers before building your map, this method might make it hard to expand your map later on. A more time-consuming alternative to this method will be mentioned.
* Run the following command in chat:
  ```
  /ctf_map e
  ```
* Click `Create New Map`.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/3364c2a7-4525-4a5d-9c7e-832a1a1e3a84)
* Next, select the area that your map will be in by either punching the nodes on the two opposite corners (similar to selecting an area with WorldEdit as mentioned above) or running the following command while standing at each corner:
  ```
  /ctf_map here
  ```
* After that, run `ctf_map e` again, scroll all the way down (ignore the fields and options), and click `finish editing`.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/d2d22f95-5e4a-4966-b964-0742fb36e929)
* Go to `<Minetest folder>/worlds/<your world name>/schems` and copy the folder `new_map`.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/d738a841-7e0a-42d2-a712-b02c6b6ceff1)
* Paste the folder into `<Minetest folder>/games/capturetheflag/mods/ctf/ctf_map/maps/`.
  
  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/f432acee-50e3-4ac1-8624-ac70cf3a5820)




### 5. Building the Map
* Find a place to build your map and start building it. You can add any structure you want. Many blocks have indestructible variants, which you can use for builds you don't want players to destroy (use the admin pickaxe to break indestructible blocks).

  ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/3a724fe8-9005-4dde-9438-36d424a2e7be)
  
* You should also add the following:
    * Indestructible blocks under the position of the flag (the flag will be added later). The minimum surface area for this indestructible platform is `5x5` blocks (the flag should be in the middle).
    * Team chests for each team. You can find them as a node in the inventory.
      
      ![image](https://github.com/CTF-handbooks/map-maker-handbook/assets/88883098/74f210ba-3b94-473a-bff8-886f8578d3d3)
    * _Optional_: ores (such as iron, diamond, or mese ores). The amount of ores for each team should be about the same to ensure that no team has an advantage (please note that mapgens such as v7 and flat come with ores).
