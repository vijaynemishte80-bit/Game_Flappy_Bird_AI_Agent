Flappy Bird AI Using Deep Q Network DQN

Overview

This project develops an AI agent that learns to play Flappy Bird using Deep Reinforcement Learning. A Deep Q Network DQN is implemented in PyTorch to enable the agent to interact with the game environment, learn from experience, and maximize rewards through trial and error.

The agent uses Experience Replay, Epsilon Greedy Exploration, and a Target Network to improve learning stability and performance.

Technologies Used

- Python
- PyTorch
- Gymnasium
- Flappy Bird Gymnasium
- Pygame
- Deep Reinforcement Learning
- DQN Deep Q Network

Key Features

- Autonomous Flappy Bird gameplay
- Deep Q Learning based decision making
- Experience Replay Memory
- Target Network Synchronization
- Epsilon Greedy Exploration Strategy
- Reward Based Learning
- GPU and Hardware Acceleration Support
- Model Saving and Loading

Project Structure

Game Environment

- Flappy Bird Gymnasium Environment
- Real time gameplay using Pygame
- Manual game testing support

Deep Q Network

- Input Layer for game state representation
- Hidden Layer with ReLU activation
- Output Layer for action prediction
- Action Space:
  - 0 = No Flap
  - 1 = Flap

Experience Replay

- Stores past experiences
- Random mini batch sampling
- Reduces correlation between training samples
- Improves learning stability

Agent Components

- Policy Network
- Target Network
- Experience Replay Buffer
- Epsilon Greedy Action Selection
- Reward Maximization

Reinforcement Learning Workflow

1. Observe current game state
2. Select action using epsilon greedy policy
3. Perform action in environment
4. Receive reward and next state
5. Store experience in replay memory
6. Sample mini batches from memory
7. Update policy network
8. Synchronize target network
9. Repeat until optimal policy is learned

Hyperparameters

Parameter| Value
Learning Rate| 0.001
Discount Factor Gamma| 0.99
Initial Epsilon| 1.0
Minimum Epsilon| 0.1
Epsilon Decay| 0.995
Replay Memory Size| 50000
Mini Batch Size| 64
Reward Threshold| 1000
Network Sync Rate| 1000

Training Features

- Experience Replay Memory
- Bellman Equation Based Q Value Updates
- Mean Squared Error Loss
- Adam Optimizer
- Target Network Synchronization
- Exploration and Exploitation Balance

Model Architecture

Input State

↓

Fully Connected Layer

↓

ReLU Activation

↓

Output Layer

↓

Q Values for Available Actions

Results

The DQN agent learns optimal gameplay strategies through continuous interaction with the Flappy Bird environment. Over time, the agent improves obstacle avoidance and survival duration, achieving higher rewards without human intervention.

Applications

- Game AI Development
- Autonomous Decision Making
- Reinforcement Learning Research
- Robotics Control Systems
- Intelligent Agent Design

Future Improvements

- Double DQN
- Dueling DQN
- Prioritized Experience Replay
- Deep Neural Network Architectures
- Multi Agent Reinforcement Learning
- Performance Visualization Dashboard

Author

Developed as a Deep Reinforcement Learning and Game AI Project using PyTorch and Gymnasium.
