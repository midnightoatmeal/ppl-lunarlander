# PPO Agent for LunarLander-v2

This project trains a reinforcement learning agent using Proximal Policy Optimization (PPO) to land a spacecraft in OpenAI Gym's LunarLander-v2 environment.

The agent was trained using [Stable-Baselines3](https://github.com/DLR-RM/stable-baselines3) and deployed to the [Hugging Face Hub](https://huggingface.co/midnightoatmeal/ppo-LunarLander-v2).


---

## Algorithm: PPO (Proximal Policy Optimization)

- On-policy RL algorithm
- Optimizes clipped surrogate objective
- Learns both policy and value function

---

## Environment: LunarLander-v2

- State space: 8D continuous
- Action space: Discrete (4 actions)
- Rewards:
  - +100 to +140 for safe landing
  - -100 for crashing
  - Bonus for efficiency & leg contact

---

## Results

- **Mean reward**: ~259  
- **Std reward**: ~48  
- Evaluated over 10 deterministic episodes

---

## Stack

- Python
- Gymnasium
- Stable-Baselines3
- Hugging Face Hub
- `huggingface_sb3` for packaging and deployment
