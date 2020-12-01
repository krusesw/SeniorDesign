# Reinforcement Learning (RL)

We will be implementing reinforcement learning when designing our first person shooter video game. Reinforcement learning 
is a commonly used machine learning technique. We have learned implementation with classic style games such as chess, tic-tac-toe,
and the classic 8-puzzle. Using our knowledge, we will be creating bot controllers for movement and individual contact. 

Generalization is crucial when designing a AI that will gather data and make increasingly better choices throughout combat. Stored
gameplay data is consistently gathered for gameplay decision analysis. Therefore, we can use a premade reinforcement learning library, 
compatible with the Unreal Engine, to sculpt agent behavior through a combination of a neural network and learning models. 

## Reward and Penalty Policies
Our agent, or bot, within the first person shooter game, will learn to acheive its goal in an uncertain, somewhat simple environment
(arena). This small environment will limit the agent's trial and error for coming up with a sufficient solution of damaging the player
and navigating the arena.The AI bot will be given rewards for shooting closely to the player, landing a shot, dodging the player's shots, and 
ultimately defeating the player eventually. (Can't be too easy or too challenging). The RL will produce penalties when the bot is shot,
comes to a stalemate in movement or shooting not relatively close to the player. Therefore, the bot's goal is to maximize rewards and
limit penalties. We, as the AI and game designers, will set the reward policy. These can be classified as the rules, or limits, within
the game. We may give the AI relatively small suggestions for how to find and shoot the player, but it will be up to the bot to truly 
find its path to victory. Therefore, the AI must perform tasks to maximise reward policy beginning with little knowledge and accumulating
data throughout battle.

## Key Elements

### Agent
Train a bot to track movement and combat decisions. This agent is a program that tracks user movement and combat data, then makes 
decisions on the data accumulated.

### Environment
Arena based game.

### Action
Actions provide methods for the agent to interact and alter the environment, therefore transferring between states. In our instance, rewards are given by movement in arena, and landing 'shots', or causing damage, on the user. 

We will use assessment to find which actions minimize loss and increase agent benefits.

### Rewards
The reward function describes agent behavior. Our rewards will be defined by how easily our agent will defeat a player. Using movement and combat data, the rewards will be ever-changing from user data. The rewards can then be considered continuous and differentiable. 

## Articles
https://www.analyticsvidhya.com/blog/2017/01/introduction-to-reinforcement-learning-implementation/ \
https://www.guru99.com/reinforcement-learning-tutorial.html \
https://neptune.ai/blog/best-reinforcement-learning-tutorials-examples-projects-and-courses \
https://www.researchgate.net/publication/224206784_Reinforcement_Learning_in_First_Person_Shooter_Games 
