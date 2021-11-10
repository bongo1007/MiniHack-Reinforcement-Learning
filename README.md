# Reinforcement-Learning

## Authors
* Michael Gomes
* Tristan Le Forestier
* Jesse Bristow
* Goolam Fareed Bangie


Reinforcement learning is a machine learning training strategy that rewards desirable behaviors while penalizing undesirable ones.
A reinforcement learning agent can perceive and comprehend its surroundings, act, and learn through trial and error in general. 

In this project we attempt to apply reinforcement learning algorithms together with deep learning in order to solve a game in the minihack environment which is built upon the NLE(NetHack Learning Environment) and the gym environment as well. 

According to the minihack docs, "MiniHack is an environment creation framework and accompanying suite of tasks that is based on NetHack, one of the hardest games in the world. With this tool, engineers can easily create a universe of tasks that challenge modern RL methods and are targeted at specific problems within RL". 

The game that we are required to train our agent to learn is the MiniHack-Quest-Hard-v0. This game involves multiple sub tasks in order to reach the goal including navigation through a maze, picking up objects of interest that are needed at later stages, crossing a lava river with one of the objects that were picked up before as well as killing a monster with the wand of death that would also need to be picked up in the environment prior to using the wand.

The two algorithms that we made use of:
## Valued Based Method
* Deep Q learning network or DQN for short

The environment can be treated exactly like a normal gym environment after running the following commands in the order that they appear
* !sudo apt-get install -y build-essential autoconf libtool pkg-config \
    python3-dev python3-pip python3-numpy git libncurses5-dev \
    libzmq3-dev flex bison
* !git clone https://github.com/google/flatbuffers.git
* !cd flatbuffers && cmake -G "Unix Makefiles" && make && sudo make install
* !pip install cmake==3.15.3
* !pip install nle==0.5.2
* !pip install "nle[agent]"

The exclamation marks before the command are needed for running these installs in the notebook that is being used for the project

**NOTE**
There is only a single dqn notebook. This notebook can be used to run all 3 of the different agents. In order to train a model 
two models need to be initialised like in the get_avg_reward_for_multiple_runs() method, then these two models can be passed 
to the learn_model() method in order to learn them. In order to learn the movements only model, the first model passed to the 
learn_model() method must only contain 4 output neurons. In order to learn the limited actionspace model, the first model passed to the 
learn_model() method must contain 18 output neurons. In order to learn the random model, the variable RANDOM_AGENT(it's just 
above the learn_model method) must be set to True.

## Policy Gradient Method
* Actor Critic or AC for short

The environment can be treated exactly like a normal gym environment after running the following commands in the order that they appear
* !sudo apt-get install -y build-essential autoconf libtool pkg-config \
    python3-dev python3-pip python3-numpy git libncurses5-dev \
    libzmq3-dev flex bison
* !git clone https://github.com/google/flatbuffers.git
* !cd flatbuffers && cmake -G "Unix Makefiles" && make && sudo make install
* !pip install cmake==3.15.3
* !pip install nle==0.5.2
* !pip install "nle[agent]"

The exclamation marks before the command are needed for running these installs in the notebook that is being used for the project

