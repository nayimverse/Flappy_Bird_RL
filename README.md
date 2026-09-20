# Flappy Bird RL

A Flappy Bird reinforcement-learning project using Gymnasium, `flappy-bird-gymnasium`, Pygame, and a PyTorch deep Q-network (DQN). It includes a manual keyboard-controlled game loop and an agent that can train or evaluate a policy.

## Requirements

- Python 3.9 or newer
- A desktop environment capable of opening a Pygame window
- PyTorch
- PyYAML

## Installation

```bash
python -m pip install gymnasium flappy-bird-gymnasium pygame torch pyyaml
```

## Run

```bash
python flappy_bird_RL.py
```

Press **Space** to flap. Close the game window to stop the program.

## Train or Evaluate the DQN Agent

Train the agent with the parameter set defined in `parameters.yaml`:

```bash
python agent.py flappybirdv0 --train
```

Evaluate the saved model with rendering enabled:

```bash
python agent.py flappybirdv0
```

Training logs and model checkpoints are written to `runs/` and are ignored by Git.

## Project Structure

- `flappy_bird_RL.py` - launches the environment and handles keyboard input.
- `agent.py` - trains or evaluates the DQN agent.
- `dqn.py` - defines the neural network used by the agent.
- `experience_replay.py` - implements the replay memory buffer.
- `parameters.yaml` - stores the training hyperparameters.
- `flappy_bird_rl/` - project directory reserved for additional RL code.
