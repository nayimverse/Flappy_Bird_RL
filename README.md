# Flappy Bird RL

A simple interactive Flappy Bird environment built with Gymnasium, `flappy-bird-gymnasium`, and Pygame. The player controls the bird manually while the environment exposes the reinforcement-learning interface.

## Requirements

- Python 3.9 or newer
- A desktop environment capable of opening a Pygame window

## Installation

```bash
python -m pip install gymnasium flappy-bird-gymnasium pygame
```

## Run

```bash
python flappy_bird_RL.py
```

Press **Space** to flap. Close the game window to stop the program.

## Project Structure

- `flappy_bird_RL.py` - launches the Flappy Bird Gymnasium environment and handles keyboard input.
- `flappy_bird_rl/` - project directory reserved for additional RL code.
