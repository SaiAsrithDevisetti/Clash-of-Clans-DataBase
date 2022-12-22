# Query 1
## Retrive the number of townhalls with gold > 3000000
From the table TownHall, we get the players with gold greater than 3000000 <br>
Uses: We get the players who have more gold, we can use it for clan selection<br>
### SELECT count(*) FROM TownHall WHERE Total_Amount_of_Gold > 300000;

# Query 2
## Retrive the Army item with max hitpoints
In the table Army, we select the item with max hitpoints <br>
Uses: Enables us to select them or not for a battle<br>
### SELECT Name_of_the_itemorBuilding FROM Army WHERE Hitpoints = (SELECT MAX(Hitpoints) FROM Army);             

# Query 3
## Retrive the player with maximum number of Session Points
From the village base table, we get the session points <br>
Uses: We get the data of the season of the game<br>
### SELECT VillageID FROM VillageBase WHERE Sessionpoints = (SELECT MAX(Sessionpoints) FROM VillageBase); 

# Query 4
## Retrive the number of builders that are free
From the table builder hut, we get the status of the builder<br>
Uses: Enables us the chance to make updates<br>
### SELECT count(*) FROM BuilderHuts WHERE Status = 'Sleeping';

# Query 5
## Retrive the number of spells and troops that are unlocked and not yet updated
From the Unlock the troop or spell table we get the data of troops and spells that can be updated<br>
Uses: Enables us with a vision of the further updates<br>
### SELECT count(*) from Unlock_the_trooporSpell where Current_level < Updated_level;

# Query 6
## Retrive the players having Resource portion
From the contains the table, players having resource can be obtained<br>
Uses: Can be used to select the friend, so that donation can be done<br>
### SELECT VillageID from Containsthe where Name_of_the_Item = 'Resource portion';

# Query 7
## Retrive the players info having Barbarian king
From Consists of, we get the players info having Barbarian king<br>
Uses: Enables us to select the opponent.<br>
### SELECT * from ConsistsOf where Name_of_the_itemorBuilding = 'Barbarian King';

# Update 1
## Update the Clan Name, if he changed the clan
Changes the clan name is player wishes to<br>

# Update 2
## Update the resource collector to the next level
We update all the attributes such, corresponding to the level update<br>

# Update 3
## Update the status of the portion
We use the portion, so that entry is deleted from table.<br>


