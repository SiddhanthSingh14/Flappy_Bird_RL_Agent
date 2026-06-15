# 🐦 Flappy Bird RL Agent

A Deep Reinforcement Learning project that trains an autonomous agent to play Flappy Bird using a Deep Q-Network (DQN) implemented in PyTorch.

## 🚀 Project Overview

This project explores Reinforcement Learning by training an AI agent to play Flappy Bird through trial-and-error interactions with the environment. The agent learns optimal actions by maximizing cumulative rewards and improving its survival time over successive episodes.

The implementation includes several key DQN enhancements such as Experience Replay, Target Networks, and Epsilon-Greedy Exploration to achieve stable and efficient learning.

---

## 🛠️ Technologies Used

* Python
* PyTorch
* Gymnasium
* NumPy
* YAML
* Flappy Bird Gym Environment

---

## 🧠 Reinforcement Learning Approach

### Deep Q-Network (DQN)

The agent uses a neural network to approximate the Q-value function:

Q(s, a)

where:

* s = current state
* a = action
* Q(s,a) = expected future reward

The network learns to estimate the long-term value of taking an action in a given state.

---

## ✨ Features Implemented

### Experience Replay

Stores previous experiences and samples random mini-batches during training to reduce correlation between consecutive experiences.

### Target Network

Uses a separate target network that is periodically updated to stabilize training.

### Epsilon-Greedy Exploration

Balances exploration and exploitation:

* Random actions during early training
* Increasingly optimal actions as learning progresses

### Configurable Hyperparameters

Training settings such as:

* Learning Rate
* Discount Factor (Gamma)
* Epsilon Decay
* Replay Buffer Size
* Batch Size

are managed through a YAML configuration file.

---

## 📂 Project Structure

```text
Flappy_Bird_RL_Agent/
│
├── agent.py                 # RL agent logic
├── dqn.py                   # Deep Q-Network model
├── experience_replay.py     # Replay buffer implementation
├── game_flappy_bird.py      # Training and evaluation loop
├── parameters.yaml          # Hyperparameter configuration
├── README.md
```

## ⚙️ Training Process

1. Initialize environment and DQN agent
2. Observe current state
3. Select action using epsilon-greedy policy
4. Execute action in environment
5. Store transition in replay memory
6. Sample mini-batches from replay memory
7. Update neural network weights
8. Periodically update target network
9. Repeat for multiple episodes

---

## 📈 Learning Objectives

The agent learns to:

* Avoid collisions with pipes
* Navigate through gaps
* Maximize survival time
* Achieve higher cumulative rewards

---

## ▶️ Running the Project

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Start Training

```bash
python game_flappy_bird.py
```

---

## 📊 Future Improvements

* Double DQN
* Dueling DQN
* Prioritized Experience Replay
* Model Performance Visualization
* Hyperparameter Optimization
* PPO and A2C Comparisons

---

## 🎯 Resume Highlights

* Developed a Deep Q-Network (DQN) agent in PyTorch to autonomously play Flappy Bird.
* Implemented Experience Replay, Target Networks, and Epsilon-Greedy Exploration.
* Built a configurable training pipeline with YAML-based hyperparameter management.
* Applied Reinforcement Learning principles to optimize long-term reward and gameplay performance.

---

## 👨‍💻 Author

Siddhanth Singh

GitHub: https://github.com/SiddhanthSingh14
