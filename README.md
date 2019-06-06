# DQN_CartPole


![alt text](XXX)


An application of DQN to the CartPole problem from OpenAI that I wrote as part of group project. Specifically, the same project described in the DQN_lunar_lander repo. deep Q-learning networks (DQN) are a form of deep reinforcement learning where an agent uses a neural network to approximate Q-learning in very high-dimensional spaces. For any finite Markov decision process (FMDP), Q-learning will find the optimal behavior, though in practice its applications are more limited. For this implementation, the agent consitently achieves perfect play after about 1000 episodes (about thirty minutes of training on an NVIDIA P1000 Quadro), though the results are somewhat erratic. 

Despite being a simpler problem, applying DQN to cartpole proved to be surprisingly difficult. I theorized that the was because the agent had to a find a precise equilbrium as the cartpole problem has no terminal state. The final DQN network had a topology of 54 neurons and 720 connections with two hidden layers of 24 neurons each, ReLu activation, and Adam optimization. The DQN also made use of an unlimited replay buffer, and a target network that used hard-tau updates at the end of every episode along with annealed exploration.

Despite the difficulties of the problem, the actual process coding was very informative. I was able to familiarize myself with the basic agent-environment loop as well as practicing embedding Keras into Python objects. I was also able to practice debugging and hyperparameter optimization in the context of deep reinforcement learning. 
