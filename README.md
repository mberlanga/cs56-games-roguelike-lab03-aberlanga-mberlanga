cs56-games-roguelike
====================

W14 ready! (Andrew Berls)

ASCII roguelike game

![](http://i.imgur.com/E8qA2Pt.jpg)



program internals
=================


The list of monsters is maintained in LogicEngine.java as a private variable:
```java
private Monster[][] listOfMonsters;
```
The LogicEngine.java constructor created the list:
```java
	listOfMonsters = new Monster[floorWidth][floorHeight];
```
Monsters are created in the createMonsters() method in LogicEngine.java
	called by checkAllMonsterStatus() in RogueController.java



RogueController.java is the MAIN
	branches:
		LogicEngine.java
			Deals with the state of the game and the movements of monsters and player
		RoguePanel.java
			Draw everything that appears on screen



