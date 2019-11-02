# OpenAI Baselines

High-quality implementations of reinforcement learning algorithms.

Covered material:
https://openai.com/blog/openai-baselines-dqn/
https://github.com/openai/baselines



Implementation:




**Difficulties in reproducing RL results:**
- very noisy performance
- many moving parts allow for subtle bugs

**Best practices:** based on these resources
- Compare to a random baseline
- Be wary of non-breaking bugs
- See the world as your agent does (check how the screen images are transformed - Gym: play)
- Fix bugs, then hyperparameters
- Double check the interpretations of papers (check gradients are as you expect - TensorFlow: compute_gradients)

**Algorithms:**
- DQN: A reinforcement learning algorithm that combines Q-Learning with deep neural networks to let RL work for complex, high-dimensional environments, like video games, or robotics.
- Double Q Learning: Corrects the stock DQN algorithm’s tendency to sometimes overestimate the values tied to specific actions.
- Prioritized Replay: Extends DQN’s experience replay function by learning to replay memories where the real reward significantly diverges from the expected reward, letting the agent adjust itself in response to developing incorrect assumptions.
- Dueling DQN: Splits the neural network into two — one learns to provide an estimate of the value at every timestep, and the other calculates potential advantages of each action, and the two are combined for a single action-advantage Q function.
