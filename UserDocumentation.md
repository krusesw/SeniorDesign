### Description 

```
VGAI is a project that seeks to use reinforcement learning to enhance the gameplay of a first-person shooter video game. 

The project consists of a first-person shooter demo with an enemy character controlled by a reinforcement learning artificial intelligence. 
```
 

### Getting Started/ Program Installation 
```

Download the executable file from our GitHub page https://github.com/krusesw/SeniorDesign VGAI.exe (releasing end of March 2021) 

Begin by double-clicking the downloaded file 

The executable may require you to download packages that are missing from your system for the game to work correctly. Click yes on these prompts to download and continue. 

A welcome screen and game menu will appear with an option to begin playing. 
```
 

### Gameplay 
```

The game functions similarly to other first-person shooters. The goal is to move around the map, and defeat the enemy character using your weapon, and dodge the enemy attacks. 

Every time you defeat the enemy, a new enemy will spawn in marking the start of a new round. Each new enemy will have updated play patterns based on the reinforcement learning AI. 

The rounds go infinitely high. 
```

### Controls 

The following section contains details on how to control the in-game player character.  

The actions listed can be done in parallel. For example: holding W and A will move the character forwards and to the right at the same time. 

 

Button/Action 

Description 

ESC 

Enter the in-game pause menu. 

W 

Move player character in the direction they are facing. 

A 

Move player character left of the direction they are facing. 

S 

Move player character opposite of the direction they are facing. 

D 

Move player character right of the direction they are facing. 

SPACEBAR 

Make player character jump. 

 

Move Mouse 

Moves in game first person camera. Changes the direction the player is facing. 

Left Mouse Button 

Fires the weapon. 

 

### UI 

The user interface contains two meters. One for health and one for weapon charge. 

* Health Meter 

- The health meter appears in the bottom left-hand side of the screen.  

- It displays a bar with five segments, representing the player’s five hitpoints.  

- Each time the player is hit with a projectile, their health will drop by 1 segment. 

- When this meter reaches 0, the player loses the game. 

- The health meter resets to full at the start of each round. 

* Weapon Charge Meter 

- The weapon charge meter appears in the bottom righthand side of the screen.  

- It displays a single bar that fills over the course of two seconds.  

- Once the meter is filled, the players weapon is ready to fire.  

- Once the player fires the weapon the meter will empty, and the weapon cannot be fired until the meter is full again. 


### Objectives 

This game focuses on defeating an enemy that will learn through reinforcement-based learning.  Defeat is defined as landing five total shots on the enemy. If you win, you will continue to infinite rounds until you are defeated. The reinforcement-based learning allows the enemy to accumulate knowledge over time. Therefore, each round becomes more challenging.  

Your objective is to survive as many rounds as you can. 

 

### Key Game Elements 

* AI Controlled Enemy 

 

The enemy character is controlled by a reinforcement learning artificial intelligence, that switches between different combat states dependent on the strength of those states against the player historically. 

The enemy character has a vision field of view of 150 degrees with no drop-off on distance. 

The enemy character can hear you when you are walking within a radius of 1000 distance (approximately the length of the courtyard).  

If the enemy AI perceives player footsteps, it will update its knowledge of where the player is. 

The enemy character can hear your weapon firing from a radius of 5000 distance (almost the entire map). 

If the enemy AI perceives player weapon fire, it will update its knowledge of where the player is. 

The perceived area the noise was created from becomes less accurate after 2500 distance. 

 

World 

 

The world contains a manor surrounded by light woodlands. 

The manor contains two floors (view Simplified Game Map for additional details). 

The surrounding mountains are unscalable. 

 

Simplified Game Map 

 

Floor 1 and surrounding woodlands 

 

Floor 2 

Taking a boost panel will send you over the courtyard and into the other room. 

Strategy/Tips 

The AI controlled enemy player is designed to learn player habits and adapt to overcome your gameplay style. Using the same strategy every round will in term cause the enemy AI to become better against that strategy. To achieve higher rounds, it is recommended to adapt your play habits against what the AI may have learned. 

The following are good beginning tips: 

Try not to stay in one area of the map for too many rounds. 

Try not to dodge projectiles the same way every time. 

Try to switch between aggressive (finding enemy and destroying) and defensive (waiting for enemy to find you) playstyles every few rounds. 

 
