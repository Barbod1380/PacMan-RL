
https://github.com/user-attachments/assets/20080c81-08ca-4f65-8e92-7a60b368d2f1
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

## ▶️ Running the Game
Run the following command to start the game:

```bash
python main.py
```

The AI will navigate the Pac-Man environment, attempting to maximize its score using Q-Learning.

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


## 📷 Demo (Optional)

![](https://github.com/user-attachments/assets/5b9e0535-5a86-480a-9c6f-c95ac6d1c60a)

