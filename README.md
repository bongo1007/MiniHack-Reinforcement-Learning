# Reinforcement-Learning

## Authors
* Michael Gomes
* Tristen Le Forestier
* Jesse Bristow
* Goolam Fareed Bangie


Reinforcement learning is a machine learning training strategy that rewards desirable behaviors while penalizing undesirable ones.
A reinforcement learning agent can perceive and comprehend its surroundings, act, and learn through trial and error in general. 

In this project we attempt to apply reinforcement learning algorithms together with deep learning in order to solve a game in the minihack environment which is built upon the NLE(NetHack Learning Environment) and the gym environment as well. 

According to the minihack docs, "MiniHack is an environment creation framework and accompanying suite of tasks that is based on NetHack, one of the hardest games in the world. With this tool, engineers can easily create a universe of tasks that challenge modern RL methods and are targeted at specific problems within RL". 

The game that we are required to train our agent to learn is the MiniHack-Quest-Hard-v0. This game involves multiple sub tasks in order to reach the goal including navigation through a maze, picking up objects of interest that are needed at later stages, crossing a lava river with one of the objects that were picked up before as well as killing a monster with the wand of death that would also need to be picked up in the environment prior to using the wand.

The two algorithms that we made use of is :
<ins>## Valued Based Method</ins>
* Deep Q learning network or DQN for short
* Actor Critic or AC for short
