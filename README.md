🚀 Project Overview
This project implements a Policy Gradient (REINFORCE) Algorithm to solve the CartPole problem using Reinforcement Learning (RL). The agent learns to balance a pole on a moving cart by interacting with the environment and maximizing cumulative rewards.

The CartPole environment consists of:

A cart that moves left or right.
A pole attached to the cart via a hinge.
The goal: Keep the pole balanced for as long as possible by applying correct forces.
Why Policy Gradient?
Unlike value-based methods (like DQN), policy gradient methods directly optimize the policy, making them well-suited for environments with high-dimensional or continuous action spaces.

📌 Key Features
✅ Custom-built Policy Network – A neural network that maps states to action probabilities.
✅ REINFORCE Algorithm – Implements Monte Carlo policy gradient for optimization.
✅ Baseline for Stability – Uses a value network to reduce variance in updates.
✅ Training & Evaluation – Analyzes model performance with reward tracking.

🏗️ Implementation Approach
1. Policy Network Architecture
A neural network models the policy function.
It takes the environment’s state (cart position, velocity, pole angle, pole velocity) as input.
Outputs action probabilities for moving left or right.
2. REINFORCE Algorithm
The agent plays multiple episodes and accumulates rewards.
Gradient ascent updates the policy to maximize expected returns.
Discounted rewards (γ) ensure future rewards are considered.
3. Training Process
The agent starts with random actions and improves by learning from rewards.
Over multiple episodes, the policy network adjusts weights to enhance performance.
4. Performance Evaluation
The training results show a steady improvement in the agent’s ability to balance the pole:

Episode	Total Reward
0	12.0
100	154.0
200	119.0
300	193.0
400+	500.0 (Max Score!)
✅ After training, the agent consistently achieves 500 reward points, proving mastery of the task.

📊 Results & Insights
Initially, the agent struggles, but policy optimization steadily improves performance.
The CartPole stays balanced for an extended period as training progresses.
The learning curve demonstrates the effectiveness of the REINFORCE policy gradient method.
🛠️ Technologies Used
Python 🐍
PyTorch / TensorFlow 🔥
Gym (OpenAI Gym) 🏋️
NumPy, Matplotlib 📊

📜 Conclusion
This project demonstrates how an RL agent can learn to solve the CartPole problem using the REINFORCE policy gradient method. With iterative learning, the agent achieves expert-level performance, proving that policy optimization techniques can effectively handle complex environments.
