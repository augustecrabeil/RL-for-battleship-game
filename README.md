# Overview

Our aim was to fully solve the naval battle problem using the tools provided by reinforcement learning. This was achieved in several stages:
• Implementation of an environment adapted to handling the tools
• Training an agent to optimally search for randomly placed boats
• Training an agent to optimally place boats in front of an agent applying a given strategy.
• Combine the two agents in the best possible way

# Table of Contents

- Project Structure
- Installation
- Usage
- Environnement

# Project Structure

- V1 : Simple reward function and algorithms from the Labs with very few adaptation. This implementation give no result.
- V2 : More complex reward function and simple DQN to learn from thousands of episode (very good results on a simple problem). We also have here all the part about adversarial agent.
- V3 : Attempt to add complex methods but impossible to increase the complexity of the problem.

# Installation

In the beginning of each notebook, the list of required libraries is provided in the first cell where they are imported.

# Usage

Every jupyter notebook is independant from the others. In each notebook, you have:

1) The imports of the required libraries
2) The creation of the environnement
3) The training of the agent
4) The results of our models

You can execute these different cells in this order and you will get our results.

# Environnement

We fully reimplemented the battleship game (in particular with the .step(), .reset() functions, etc.). For the design of our environment, we decided to model the board as an n × n array. Each value of the array represents the state of the corresponding case on the board: 0 for a case that has not been touched, −1 for a “miss” case, case targeted by the player but where there was no boat and 1 for a “touched” boat by a move from the player.

