# Pong
This repo contains the code to solve the Pong environment using Deep Q-learning [DQN]

# Description
![alt text](https://github.com/kwquan/Pong/blob/main/pong_sample_2.jpg)

In this notebook[Pong.ipynb], we shall solve the Pong environment using Deep Q-learning. \
Most of the code is derived from this article here[https://towardsdatascience.com/deep-q-network-dqn-i-bce08bdf2af]. \
I removed parts of it to make it simpler & added my own explanations in the notebook. \
Also, I used this on the latest Pong version[V5]

Aim: Pong consists of 2 paddles, the left paddle is controlled by the game AI while the right paddle is controlled by our agent \
The objective of each player is to hit the ball past the opponent's paddle. \
Doing so will result in a reward=1. \
On the contrary, losing to the opponent will result in a reward=-1. \
Episode terminates when either player reaches a score of 21. 
     
Observation space: \
&nbsp;             We changed the observation space to return a 4x84x84 state \
     Action space: \
&nbsp;             We only consider 6 useful actions with similar pairs \
&nbsp;             As mentioned in the article, the actions are [‘NOOP’, ‘FIRE’, ‘RIGHT’, ‘LEFT’, ‘RIGHTFIRE’, ‘LEFTFIRE’] with 
&nbsp;             3 of the 6 being redundant (FIRE is equal to NOOP, LEFT is equal to LEFTFIRE and RIGHT is equal to RIGHTFIRE) \
     Rewards: \
&nbsp;               1 if ball hit past opponent's paddle \
&nbsp;               -1 if ball hit past agent's paddle \
&nbsp;               0 otherwise
         
        
# Documentation
https://www.gymlibrary.ml/environments/atari/pong/           
