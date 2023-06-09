## Max and Lucia’s Quest for the Holy Grilled Cheese
CSE 4410 March 2, 2023 
### We’re Trying
Aldo Avalos, Omar Valle, Kevin Villatoro, Victor Vera, Alex Dragoi, Tim Chester
## Devlog 1
Welcome to the beginning of development for our game! As you may know, we are making a top down JRPG in the style of the Mario and Luigi games. We are aiming to have top down exploration, and an active, timing based system for the combat of the game.
Firstly we were able to create the tileset for the starting area. This means that we were able to create the visuals for the starting area for our game. We had to use Unity’s layer system in order to stack visuals for objects like a house and trees on top of the ground. This same layering system will allow us to create colliders only for certain parts of the visuals like walls or objects. Something we’re trying to implement is adding collision to some of the tiles. Objects in our environment like the river, house, trees, hills will need collision so that our character does not fall out of the map and will make the level design look great.

Next, we also created a player character that can be moved with W-A-S-D. They are fully animated to move up, down, left, and right. Every frame, Unity engine checks for whether the player has pressed the buttons for movement. If they have, then Unity applies a force in that direction using its own rigid body 2d system. On top of this, an attack was added to the player character. In the animation for the attack, a child object is manipulated to appear in the direction of the attack. If this object overlaps with an enemy, the enemy can react to it in some way. We will implement a function that allows a transition to the battle scene when an enemy is attacked.

Speaking of enemies, an enemy script was added to allow for random movement. This enemy will move in a random direction after a certain number of seconds. On top of this, there is a 50% chance that it will not move at all. Hopefully this allows for an unpredictable and organic feeling enemy.
A partner was added. This will be our Lucia, or Max, depending on who you want to play as, because you will be able to switch between the two. This partner will automatically follow you as you explore the world. You can also press left alt to switch between the two characters. 
