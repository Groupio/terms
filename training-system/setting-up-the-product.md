---
cover: .gitbook/assets/New Project (7).png
coverY: 0
---

# 🛠️ Setting up the product

<figure><img src=".gitbook/assets/New Project (4).png" alt=""><figcaption></figcaption></figure>

This will guide you through how to set up the training system.&#x20;

## Inserting The Product

1. Download the file from Parcel
2. Open the game you wish to add the training system to in Roblox Studio

If you wish to use the Groupio Plugin for your setup, go to [Using the Groupio Plugin](setting-up-the-product.md#using-the-groupio-plugin). However, if you do not want to use the plugin to set it up go to [without the groupio plugin](setting-up-the-product.md#without-the-groupio-plugin).

### Using The Groupio Plugin

3. Click on 'File Setup' and select the Training System file (this may be named 'im31bxcqb55ff75hx58pan8ayw4f' )
4. If using 'Manual Setup' or 'Automatic Setup', insert the file by right-clicking workspace then select the option. It is recommended to do a Manual Setup if you have already inserted the file. [**Skip to Required Settings**](setting-up-the-product.md#required-settings) **if you used File Setup**

### Without the Groupio Plugin

3. Right-click on 'Workspace' then click Insert from the file.
4. Select the Training System file (This may be named 'im31bxcqb55ff75hx58pan8ayw4f' )
5. Move the contents of the folders into the correct services (E.g. all the contents of ReplicatedStorage should be moved into ReplicatedStorage, as the picture below shows)

<figure><img src=".gitbook/assets/image (21).png" alt="A picture of Replicated Storage with the Training System set up. Inside it has &#x27;TrainingConfig&#x27;, &#x27;TrainingSystem&#x27; and &#x27;TrainingSystemEvents&#x27;"><figcaption></figcaption></figure>

6. Open the 'TrainingSystem' module script

## Required Settings

6. If you do not already have the 'TrainingSystem' module script open for the settings, open it in ReplicatedStorage.
7. Set the 'GroupId' to the Id of your Roblox Group. This can be found in the link: https://www.roblox.com/groups/**GroupId**/**GroupName**#!/about
8. Set the 'TrainerRank' to the lowest rank id you want to have trainer abilities
9. Set the 'HostRank' to the lowest rank id you want to have host abilities
10. Set the 'SupervisorRank' to the lowest rank id you want to have supervisor abilities
11. Set 'Name' to the Name of your Roblox Group, this will be the name used for {name} in information messages.

```lua
local GroupId = 34362992 -- Id of your Roblox Group

local TrainerRank = 10 -- Minimum Rank Id that should be able to train players
local HostRank = 50 -- Minimum Rank Id that should be able to host trainings
local SupervisorRank = 100 -- Minimum Rank Id that should be able to supervise trainings.

local Name = "Place Name Here!" -- The place name. 
```

12. Set up the Doors, TeleportLocations and Cameras. A guide on how to do this is shown in [Customization of the Product. ](customization-of-the-product.md)

