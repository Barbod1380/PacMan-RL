# Pac-Man Game with Q-Learning
## 🕹️ Overview
This project implements a simple **Pac-Man game** where the AI agent learns to navigate using **Q-Learning**, a Reinforcement Learning (RL) algorithm. The agent improves its decision-making over time by interacting with the game environment and receiving rewards.


## 🚀 Features
- **AI-controlled Pac-Man** using Q-Learning
- **Customizable game environment**
- **Exploration vs. Exploitation balance** for optimal learning
- **Reward-based learning mechanism**
- **Randomized starting positions** for better generalization

## 🛠 Installation
To run the project, ensure you have Python installed. Then, install the required dependencies:

```bash
pip install numpy pygame
```

## 🤖 How Q-Learning Works
Q-Learning is a reinforcement learning algorithm that helps the AI learn the best actions to take in a given state. The core idea is:

1. **Initialize a Q-table** to store state-action values.
2. **Choose an action** based on an exploration-exploitation strategy.
3. **Perform the action** and receive a reward.
4. **Update the Q-value** using the Bellman equation:
   
   ```
   Q(s, a) = (1 - α) * Q(s, a) + α * (reward + γ * max(Q(s', a')))
   ```
   where:
   - `s` = current state
   - `a` = action taken
   - `s'` = new state after action
   - `α` = learning rate
   - `γ` = discount factor

5. **Repeat the process** until the AI learns optimal actions.


## 📷 Demo
<img src="https://github.com/user-attachments/assets/48816dc1-11c7-4a9c-9331-93a907a53207" alt="PacMan-Demo" width="500" />


## NOTES:
- First, this Pac-Man version doesn't contain any ghosts (maybe in the future).
- Second, we train this model many times across 10 different maps. However, since there are 3^12 different states, there will be some states that the model hasn't encountered before, which might lead to incorrect actions. You can increase the model's performance by loading the Q-matrix and training it further (this is just one way to improve the model).

