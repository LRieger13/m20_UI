# **m20-server**
Trying my hand at building a service for a game engine. Going to base it around a d20 tabletop game. Once the restful service is up i'll build a UI for it later. For now this is just an exercise of building a service to compliment a tabletop game.

## *Update* 
###### 10/06/2019 
I want to make this into more of an `adventure combat card game` if that makes any sense... Let's see what the wifey can do on a front end. May make some items for Hacktober 2019. May fall into doing some other things. Just not sure yet what is in store. 

Another thing I would like to do this switch the resources out for SQLite and knex. Muwahahahahahaha. 

## **Endpoints**
* get localhost:8080/tile to generate a tile to play. 
* get localhost:8080/scavenge/?level=5 to generate a scavenge at level 5. 
* get localhost:8080/craftableItemList to get a list of all craftable items. 
* post localhost:8080/findCraftableItem to get a list of all items craftable from a { materials: array } body.

# **M20**
## *Rules*

## **Gameplay**
>* You spawn in an empty tile devoid of all monsters.
>* When ready each player pays an action point to spawn a tile. 
>* Once the tile is spawned the leader of the group (or the one with the laptop) describes the buildings and vehicles to the players. 
>* Do not reveal what is inside the buildings or vehicles just the name and size of building. 
>* At this point players with scouting have the chance to sneak into a building.
    * If sneak is successful players get to know what is in the building. 
    * If sneak is critically successful go ahead and steal an item as well.
>* If players choose to enter the building pay 1 AP each to break in. 
>* Monsters of 1 type all attack together people entering the building. 
>* Each player pays an action point and rolls for damage to target monster. 
>* Once all players have rolled one player rolls for damage from monster. Rolling player is dealt that damage. 
    * Special note here have fun. If something bad is going to happen. Feel free to jump in front of the monster and take the damage yourself.
>* Rinse and repeat until the monster is dead or you are. 
    * If the monster dies go ahead and split the XP among attackers.
    * If player dies they pass out on the floor. More on this later. 
>* Once all monsters have been cleared from building.
    * Pay an AP to loot building. The player that pays gets to dole out the loot or keep it all.
    * Feel free to sleep in the empty building.
        * If enemies are still alive on the tile lose 20 HP and 1 AP for sleeping in shifts. 
        * If the tile is empty you sleep well. Good chance to get crafting done. 
>* If all players are passed out the monsters lose interest. You wake back up in the spawn point regenerated. 
    * For a harder experience feel free to roll to see if you keep your current inventory. 

## **Combat**
Upon entering a structure. Draw the number of monster cards necessary to fill the building. Since all monsters are territorial they attack immediately
If your health reaches 0 you lose your current equipment and faint until someone comes to rescue you.

Roll 1 D20 for each combat action taking place.
* 15-20 Critical successful: Not only did you complete your task. But it cost you no action points.
* 10-15 succesful: Task completed.
* 5-10 failure: Task failed.
* 1-5 Critical failure: Not only did you fail your task but it’s going to cost you something.

* On critical failure when carrying a weapon ranged jams and melee gets stuck. Roll again. 
    * Failure means weapon breaks. 
    * Success means weapon is restored and end turn.

## **Action Points**
* Each player starts at 10 action points everyday.

## **Inventory**
* Start with a 5 slot bag.
* Can  pick up better bags for inventory.
* Each level add 1 additional slot to inventory.
 
## **Structures**
Each tile has 1 structure on it.
That structure is decided at random from a pool of structures. Roll for amount of creatures in spawn.
Structure size is small, medium, or large.

General rule of thumb on structures: 
* Small structures have 2 resource and 1 enemy spawns.
* Medium structures have 4 resources and 2 enemy spawns.
* Large structures have 6 resourrces and 3 enemy spawns.

## **Stats**
Start out with a base of 1 in each category.
Maximum stat level is 10. 

>* Strength- Melee weapons
>* Marksmanship- Shoot range weapons
>* Scavenging- Gather more resources
	* Every 2 stat points is an additional resource of your choice per building cleared must be done as an action.
>* Crafting- Your crafting level must match item level to be able to make. 
    * On critical success crafting consumed 0 resources. 
    * On critical failure destroy all resources. 
>* Stamina- increase number of action points per day
	* Every 2 skill points is 1 extra action point per day
>* Scouting- The ability to sneak a peek into buildings.
    * lvl 3 you can scout a small building.
    * lvl 7 scout a medium building. 
    * lvl 10 scout a large building.
>* Salvaging- Break down an item into it's materials. 
    * Every 2 skill points is 1 material to salvage from an item. 
    
## **Resources:**
Resources are associated with a building. A hospital which is a large structure would have 3 resources that are medical supplies. Whereas a construction store which is a large structure would have 3 resources that are 1 weapon, 1 building resource, and 1 food.
The resource types are weapons, building resources, food, and medical.
Weapons:
Weapons are an item that increase your combat effectiveness. This is also broken down in to 3 categories which are common weapons, uncommon weapons, and rare weapons.
* Common weapons just add a maximum of 1 to your roll.
* Uncommon weapons add a maximum of 2 to your roll and have a trait associated with them.
* Rare weapons add a maximum of 3 to your roll and have a trait associated with them.

###### Example Common:
* Shovel
* +1 to rolls.
* Requires 1 strength

###### Example uncommon:
* 12 ga shotgun
* +2 to rolls
* Requires 2 marksmanship
* targets two enemies at once.

###### Example rare:
* Chainsaw
* +3 to rolls.
* You are a mad man target 4 enemies at once.
* Requires 5 strength.

## **XP**
Even split of xp between attackers unless 1st attacker kills creature all xp goes to that player.
###### *Level*
For each level gain that level amt in skill points
* 1-2: 200xp
* 2-3: 300xp
* 3-4: 400xp
* 4-5: 500xp
* 5-6: 600xp
* 6-7: 700xp
* 7-8: 800xp
* 8-9: 900xp
* 9-10: 1000xp

###### *Health*
* Level 1- 100
* Level 2- 120
* Level 3- 140
* Level 4- 160
* Level 5- 180
* Level 6- 200
* Level 7- 220
* Level 8- 240
* Level 9- 260
* Level 10- 280

###### *Characters*
* Each player starts with 10 stats spread into whatever skill they want.
* Every level put that number of stat points into stats. So level 2 is a 2 stat point gain. Level 3 is a 3 stat point gain. 
