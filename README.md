# SnakeAI

The SnakeAI is a reinforcement learning model designed to play the classic Snake game. The AI uses a neural network to learn the optimal policy for navigating the snake towards the food while avoiding collisions.

## Overview

- **Environment**: The AI operates in a custom Snake game environment. The game involves navigating a snake around a grid, consuming food, and growing in length. The game ends if the snake collides with the boundaries or itself.
- **Model**: The core of the AI is a neural network-based Q-learning model. The network takes the game state as input and outputs Q-values for each possible action.
- **Agent**: The agent interacts with the game environment, selects actions based on the current policy, and updates the policy using the REINFORCE algorithm.
- **Training**: The agent is trained by playing the game repeatedly. After each game, the agent updates its policy based on the rewards received and the actions taken.

## Files

- `agent.py`: Contains the implementation of the agent, including the policy network, training loop, and action selection mechanism.
- `game.py`: Implements the Snake game environment, including the game logic, rendering, and interaction mechanisms.
- `helper.py`: Provides utility functions, including a function to plot the agent's performance over time.
- `model.py`: Contains the neural network architecture for the Q-learning model and the training mechanism.

## Getting Started

- Clone the repository.
- Install the required libraries and dependencies.
- Run the agent.py script to train the agent and watch it play the game.

## Training Process

The training process involves the following steps:

- **Interaction**: The agent interacts with the game environment, selecting actions based on its current policy.
- **Policy Update**: After each game, the agent updates its policy using the REINFORCE algorithm. The goal is to increase the probability of actions that resulted in high rewards and decrease the probability of actions that led to low rewards.
- **Evaluation**: The agent's performance can be visualized using the plotting function in helper.py, which shows the agent's score over time.
