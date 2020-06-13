# addon-liveries
(Couldn't post it to #development:tutorials please move)

I was looking for a way to add liveries "properly" by making a .yft file, couldn't find a guide and if I asked around everyone said I should just add the livery to the .ytd file as a texture.

Finally figured it out and thought someone would find this guide helpful! :)


"Credits"
![](https://i.imgur.com/PV8uzvD.png)



> **Step 1**
Download Texture Toolkit
https://www.gta5-mods.com/tools/texture-toolkit

> **Step 2**
Download my .yft and .dds files
https://github.com/Curiosity-GitHub/addon-liveries

> **Step 3**
Make your livery.
Use the .dds file you downloaded (Make sure to not change the file name or the picture size)

> **Step 4**
Open Texture Toolkit and *Load* the .yft file you downloaded.
![](https://i.imgur.com/1sUu5kT.png)


> **Step 5**
Import the .dds file you edited to your liking. (!MAKE SURE THE FILE NAME IS elegy1_livery1.dds!)
![](https://i.imgur.com/mKx5Phx.png)

> **Step 6**
Export your new livery.yft file (Name the file CARSPAWNCODE_livery1.yft)
*(Examples: gtr_livery1.yft, skyline_livery1.yft , rs7.yft etc.)*
![](https://i.imgur.com/81t8v2J.png)


> **Step 7**
Drop the car_livery1.yft file into your vehicle's stream folder

> **Step 8**
Modify your carcols.meta


```
<Item>

          <modelName>car_livery1</modelName>

          <modShopLabel>BLANK</modShopLabel>

          <linkedModels/>

          <turnOffBones />

          <type>VMT_LIVERY_MOD</type>

          <bone>chassis</bone>

          <collisionBone>chassis</collisionBone>

          <cameraPos>VMCP_DEFAULT</cameraPos>

          <audioApply value="1.00000000"/>

          <weight value="0"/>

          <turnOffExtra value="false"/>

          <disableBonnetCamera value="false"/>

          <allowBonnetSlide value="true"/>

        </Item>
```
![](https://i.imgur.com/1PpPvvx.png)

> **Step 9**
Modify your vehicles.meta < flags > - Remove the flag "FLAG_HAS_LIVERY".

**IF YOU HAVE "FLAG_HAS_LIVERY" THEN REMOVE IT**

`      < flags >FLAG_SPORTS FLAG_AVERAGE_CAR< /flags >`
