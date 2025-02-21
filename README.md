# Artificial-Intelligence-SC3000-
CartPole-v1 Reinforcement Learning with Q-Learning

## Overview

This project implements a reinforcement learning (RL) agent using Q-learning to solve the CartPole-v1 environment from OpenAI Gym. The goal of the agent is to balance a pole on a moving cart for as long as possible by learning an optimal policy through trial and error.

## Environment

CartPole-v1

### Action Space: Discrete (2)

0 - Push cart to the left

1 - Push cart to the right

### Observation Space: Continuous (4)

Cart position

Cart velocity

Pole angle

Pole velocity at tip

### Reward: +1 for every time step the pole remains upright

### Episode Termination:

Pole angle exceeds ±12 degrees

Cart position moves more than ±2.4 units from center

Episode length reaches 500 steps

## Implementation Details

Algorithm: Q-learning

State Discretization: The continuous observation space is discretized into a finite number of bins to enable tabular Q-learning.

Q-table: A table storing action-value estimates for state-action pairs.

## Exploration Strategy:

Epsilon-greedy policy

Decreasing epsilon over episodes to balance exploration and exploitation

## Hyperparameters:

Learning rate (alpha)

Discount factor (gamma)

Epsilon decay schedule

Number of bins per observation dimension

## Installation

### Prerequisites

Ensure you have Python installed, along with the required libraries:

pip install numpy gym matplotlib

## Results

The agent learns to balance the pole through Q-learning.

Training performance is visualized using reward curves.

The trained agent is evaluated to measure its stability and performance.

## Future Improvements

Implement function approximation using deep Q-networks (DQN) for better generalization.

Fine-tune hyperparameters for improved performance.
