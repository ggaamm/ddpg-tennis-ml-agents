[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"


# Project 3: Collaboration and Competition

### Introduction

For this project, The agents will learn racket ball [Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) environment.

![Trained Agent][image1]

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1.  If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01.  Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 24 variables per agent corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation.  Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. In total there are 4 actions for two agents. 

The task is episodic, and in order to solve the environment, any agent must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

- After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
- This yields a single **score** for each episode.

The environment is considered solved, when the average (over 100 episodes) of those **scores** is at least +0.5.

### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)

2. Place the file in a folder, can be named as `p3_collab-compet/` folder, and unzip (or decompress) the file. 

In addition, the necessary libraries are:

3. Python 3 and Pytorch https://pytorch.org/

4. numpy, matplotlib

5. Unity ml agents:https://github.com/Unity-Technologies/ml-agents

### Instructions

Follow the instructions in `Tennis.ipynb` to get started with training your own agent!
The actor critic neural network source code is `model.py`
The agent and replay buffer is in `agent.py`
The saved model parameters of 2 agents for actor and critic network can be found in `checkpoint_actor_tennis.pth` and `checkpoint_critic_tennis.pth` forms
