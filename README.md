# Reinforcement-Learning

In the notebook Q_learning.ipynb you can find a basic implementation of the Q-learning algorithm using open AI gym and numpy.

# Frozen Lake

The environment used for training is the frozen lake environement that you can explore here : https://gym.openai.com/envs/FrozenLake-v0/

In short it's a 2D grid (4 x 4 = 16 cells) like the following :

SFFF       

FHFH       

FFFH       

HFFG       

(S: starting point, safe) (F: frozen surface, safe) (H: hole, fall to your doom) (G: goal, where the agent must get)

The agent must learn to reach the goal cell (G) starting from the cell (S) and taking only the frozen cells (F) and avoiding the holes (H). 

The difficulty of the task lies in the stochastic nature of the environment. As a matter of fact, when an agent takes a step (up, down, left, right), it is not sure about where it ends up. In fact since the floor is frozen, the agent might slip into a neighboring cell !  

In the Q_learning.ipynb notebook we reach a success rate of ~ 76%
