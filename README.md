# **m20-server**
Trying my hand at building a service for a game engine. Going to base it around a d20 tabletop game. Once the restful service is up i'll build a UI for it later. For now this is just an exercise of building a service to compliment a tabletop game.

## *UPDATE*
###### 02/28/2020
I ended up using this idea as a template for a project I did in my Web Interface Design course during my Bachelor's program. Feel free to peruse and lemme know what ya think of the first draft. Already have some ideas on how to imprpove on some parts that aren't so modern [ like the scroll boxes on the rules page ].

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
