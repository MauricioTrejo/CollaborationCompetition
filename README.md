# Collaboration and Competition

Playing tennis with Reinforcement Learning.

## Index

1. [Project](#project)
2. [Requirements](#requirements)
3. [Installation](#installation)
4. [Files](#files)
5. [Acknowledgement](#acknowledgement)

<a name="project"></a>
## Project

In this environment, two agents control rackets to bounce a ball over a net.

[![IMAGE ALT TEXT](tennis.gif)]

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores. This yields a single score for each episode. The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.

<a name="requirements"></a>
## Requirements

Packages needed for this project:

tensorflow 1.7.1 and [torch 0.4.0](https://pytorch.org/get-started/previous-versions/)

<a name="installation"></a>
## Installation

In order to run this project is important to set a python environment, you can follow the instructions [here](https://github.com/udacity/deep-reinforcement-learning#dependencies). 
  - There are 2 ways to install tensorflow 1.7.1 in your environment, one is with conda and the other is with pip (which is the one we recommend since conda installer has problems with this version of tensorflow)
  - Also, is important to note that the installation of torch has to be from [here](https://pytorch.org/get-started/previous-versions/), otherwise, neither pip nor conda will find the version.

<a name="files"></a>
## Files

- [agent](https://github.com/MauricioTrejo/CollaborationCompetition/blob/master/agent.py) is the py file containing the agent.
- [model](https://github.com/MauricioTrejo/CollaborationCompetition/blob/master/model.py) is the py file containing the neural network.
- [weights](https://github.com/MauricioTrejo/CollaborationCompetition/blob/master/weights.pth) contains the weights of the trained agent.
- [Report](https://github.com/MauricioTrejo/CollaborationCompetition/blob/master/Report.ipynb) contains the report of the agent training.
- [data/Tennis...](https://github.com/MauricioTrejo/CollaborationCompetition/tree/master/data/Tennis_Windows_x86_64) is Unity's environment.
- [python/](https://github.com/MauricioTrejo/CollaborationCompetition/tree/master/python) has necessary files for Unity's environment.
- [banana_collector](https://github.com/MauricioTrejo/CollaborationCompetition/blob/master/banana_collector.gif) is a gif with the environment of the project.

<a name="acknowledgement"></a>
## Acknowledgement

We want to thank [Unity](https://unity.com/) and [Udacity](https://www.udacity.com/) for the environment and training to solve this project.
