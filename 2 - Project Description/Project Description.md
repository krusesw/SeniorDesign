
## Project Description
For our Senior Project, we will be creating a single player game that utilizes Artificial Intelligence to create a more immersive and challenging experience for the player. The game will be a 3D First Person Shooter, meaning the combat system will revolve around the player controlling a character from the first-person point of view. The combat will consist of the player and the artificial intelligence using projectiles to fire at one another, and each time a projectile hits someone it reduces their health bar by a fixed amount until one reaches 0, meaning the victor is the one remaining with health left. The arena will be a small walled in area with a few obstacles that both characters can use to hide behind. The players can move in the X and Y direction but will not be able to jump. We will be using Unreal Engine to create this game. 

## Project Motivations
Our motivation behind using artificial intelligence is that it will allow us to create an immersive and challenging experience for the player. The AI will be able to learn from the player in order to adapt and create a more in depth and personalized experience. We will be using a feed forward back propagation neural network. This means that the AI will receive certain parameters as inputs for its decision making, and it will go through “neurons” that will apply weights to these input values in until it produces a certain acceptable output.

## Back Propagation Neural Network
We have 3 algorithms determining the movement of our AI, one will determine lateral movement and one will determine angular movement, such as which way the AI is facing. The final will determine whether to attack or not.
* The inputs of our lateral movement AI is going to consist of an (x, y) coordinate of the player, an (x, y) coordinate of the AI, and from this we can calculate the distance between the two which acts as another parameter
* The outputs of our algorithm will be a magnitude to move in the X direction, and magnitude to move in the Y direction
* The inputs of our angular movement will be angle the AI is facing from the positive X axis. So a value of 30 means that it is currently facing 30 degrees to the right of the X axis. A value of -30 means it is currently facing 30 degrees to the left. All axis’s are relative to the center of the AI character. And a last value is a Boolean of whether the player is within a certain threshold to the center of the AI’s view
* The outputs will be a value to either rotate left at a fixed speed, or rotate right at a fixed speed.
* Lastly we want to determine whether the AI should attack. Inputs for this being AI health, player health, and whether the player is in the AI’s frame or not, which can be given from the previous algorithm. 
* Outputs will be whether to attack or not.
* At first we had planned on using the health of the player as a parameter but ultimately that would only needlessly complicate the algorithm and in the long run the goals of our AI are the same no matter the health of the player
Ideally these will be the only algorithms we will need. It’s possible to have it combined into one but that raises complications due to the vast array of values that our parameters can be.

## Success Metrics
For the project to beconsidered a success, it needs to be entertaining and the AI to be successful in defeating the player

#### Entertainment metric
If our game is entertaining, then players will return to the game to play again. This metric is called retention, and our exact measure of retention success is as follows:\
If 50% of players return to the game at least once and play at least 2 hours in the first week of having the game, then the game will be considered entertaining.

#### AI success
The way we will determine success of our algorithm is that for every x games the player plays, then the Algorithm won a percentage equal to:\
![equation](http://www.sciweavers.org/tex2img.php?eq=%5Cfrac%7B60%7D%7B1%2Be%5E%7B-0.1%28x-50%29%7D%7D%20&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0)
