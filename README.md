# Reinforcement-Learning-RL :
# 1. Introduction :
Reinforcement learning (RL) is an important type of machine learning concerned with how intelligent agents ought to take actions in an environment in order to maximize the notion of cumulative reward.
The idea behind Reinforcement Learning is that an agent will learn from the environment by interacting with it and receiving rewards (Negative/Positive) for performing actions.

Learning from interaction with the environment comes from our natural experiences, RL is just a computational approach of learning from action.

## 1.1 The Reinforcement Learning Problem :

The reinforcement learning problem is meant to be a straightforward framing of the problem of learning from interaction to achieve a goal. The learner and decision-maker is called the agent. The thing it interacts with, comprising everything outside the agent, is called the environment. These interact continually, the agent selecting actions and the environment responding to those actions and presenting new situations to the agent. The environment also gives rise to rewards, special numerical values that the agent tries to maximize over time. A complete specification of an environment defines a task, one instance of the reinforcement learning problem.

More specifically, the agent and environment interact at each of a sequence of discrete time steps, t=0,1,2,3,4... At each time step t, the agent receives some representation of the environment's state, ![](https://latex.codecogs.com/svg.latex?S_{t}%20\in%20S), where ![](https://latex.codecogs.com/svg.latex?S) is the set of possible states, and on that basis selects an action, ![](https://latex.codecogs.com/svg.latex?A_{t}%20\in%20A(S_{t})), where ![](https://latex.codecogs.com/svg.latex?A(S_{t})) is the set of actions available in state ![](https://latex.codecogs.com/svg.latex?S_{t}). One time step later, in part as a consequence of its action, the agent receives a numerical reward, ![](https://latex.codecogs.com/svg.latex?R_{t+1}\in%20R), and finds itself in a new state, ![](https://latex.codecogs.com/svg.latex?S_{t+1}).

<img src="https://github.com/addi-kamal/Reinforcement-Learning-RL/blob/main/images/RLproblem.png" width="700" height="350">  

## 1.2 The Reinforcement Learning Process :

To illustrate, let’s suppose that our reinforcement learning agent is learning to play Super Mario Bros as a working example. The reinforcement learning process can be modeled as an iterative loop that works as below :

<img src="https://github.com/addi-kamal/Reinforcement-Learning-RL/blob/main/images/mario.svg" width="900" height="460">  

* At step t, Our Agent receives state ![](https://latex.codecogs.com/svg.latex?S_t) and reward ![](https://latex.codecogs.com/svg.latex?R_t) from the Environment
* Based on that state ![](https://latex.codecogs.com/svg.latex?S_t) and reward ![](https://latex.codecogs.com/svg.latex?R_t), agent takes an action ![](https://latex.codecogs.com/svg.latex?A_t) : [Jump, duck or move forward]
* Environment transitions to a new state ![](https://latex.codecogs.com/svg.latex?S_{t+1})
* Environment gives some reward ![](https://latex.codecogs.com/svg.latex?R_{t+1}) to the agent

This RL loop continues until we are dead or we reach our destination, and it continuously outputs a sequence of state, action and reward.
The goal of the agent is to maximize the expected cumulative reward.


