# Multi-Armed Bandit Simulation

This repository contains coursework for a reinforcement learning assignment focusing on the Multi-Armed Bandit problem. The Multi-Armed Bandit problem is a classic example in reinforcement learning, where an agent must choose between multiple options (arms) to maximize its total reward over a series of trials.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Simulation Details](#simulation-details)
- [Results](#results)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

The Multi-Armed Bandit problem is a fundamental problem in reinforcement learning. The goal is to determine the optimal strategy for selecting between multiple actions to maximize the expected reward. Each action (or arm) provides a random reward from a distribution specific to that action. The agent's task is to balance exploration (trying out different actions to learn their rewards) and exploitation (selecting the action with the highest known reward).

## Installation

To run the simulation, you need to have Python installed along with the necessary libraries. You can install the required libraries using the following command:

``` pip install -r requirements.txt ```

## Usage

The main simulation is implemented in the Jupyter notebook `Multi_Armed_Bandit_Simulation.ipynb`. You can open this notebook using Jupyter Notebook or Jupyter Lab to explore and run the code.

``` jupyter notebook Multi_Armed_Bandit_Simulation.ipynb ```

## Simulation Details

The notebook includes the following key components:

1. **Problem Setup**: Definition of the Multi-Armed Bandit problem, including the number of arms and their respective reward distributions.
2. **Algorithms Implemented**:
   - **Epsilon-Greedy**: A simple strategy that with probability `epsilon` explores a random arm, and with probability `1-epsilon` exploits the best-known arm.
   - **UCB (Upper Confidence Bound)**: A strategy that selects arms based on their estimated value and uncertainty.
   - **Thompson Sampling**: A Bayesian approach that selects arms based on sampling from their posterior distributions.
3. **Simulation Execution**: Running the simulation over a series of trials and collecting the results.
4. **Performance Evaluation**: Analyzing the results by plotting the cumulative reward and comparing the performance of different algorithms.

## Results

The results of the simulation are visualized in the notebook through various plots:

- **Cumulative Reward**: Shows the total reward accumulated over time for each algorithm.
- **Regret**: Measures the difference between the reward of the optimal strategy and the reward obtained by the algorithm.
- **Arm Selection Distribution**: Displays how often each arm was selected by the different algorithms.

## Conclusion

The Multi-Armed Bandit simulation provides insights into the performance of various exploration-exploitation strategies. Each algorithm has its strengths and weaknesses, and the choice of algorithm can significantly impact the cumulative reward and overall performance.

## References

- Sutton, R. S., & Barto, A. G. (2018). *Reinforcement Learning: An Introduction*. MIT Press.
- Bandit Algorithms for Website Optimization: A comprehensive resource on bandit algorithms.
