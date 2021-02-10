### AI Controlled Enemy

![](https://github.com/krusesw/SeniorDesign/blob/master/13%20-%20User%20Documentation%20Game%20Manual/Manual%20Pages/enemyAI.JPG)

* The enemy character is controlled by a reinforcement learning artificial intelligence, that switches between different combat states dependent on the strength of those states against the player historically. 

* The enemy character has a vision field of view of 150 degrees with no drop-off on distance. 

* The enemy character can hear you when you are walking within a radius of 1000 distance (approximately the length of the courtyard).  

* If the enemy AI perceives player footsteps, it will update its knowledge of where the player is. 

* The enemy character can hear your weapon firing from a radius of 5000 distance (almost the entire map). 

* If the enemy AI perceives player weapon fire, it will update its knowledge of where the player is. 

* The perceived area the noise was created from becomes less accurate after 2500 distance. 
