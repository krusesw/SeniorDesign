# Reinforcement Learning

We will be implementing reinforcement learning when designing our first person shooter video game. Reinforcement learning 
is a commonly used machine learning technique. We have learned implementation with classic style games such as chess, tic-tac-toe,
and the classic 8-puzzle. Using our knowledge, we will be creating bot controllers for movement and individual contact. 

Generalization is crucial when designing a AI that will gather data and make increasingly better choices throughout combat. Stored
gameplay data is consistently gathered for gameplay decision analysis. Therefore, we can use a premade reinforcement learning library, 
compatible with the Unreal Engine, to sculpt agent behavior through a combination of a neural network and learning models. 

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
https://www.researchgate.net/publication/224206784_Reinforcement_Learning_in_First_Person_Shooter_Games \
