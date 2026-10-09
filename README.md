# Asteroids

A 2D Asteroids-style arcade game built with **Python** and **Pygame** as part of the [Boot.dev](https://www.boot.dev/) backend developer learning path.

The player controls a spaceship, avoids incoming asteroids, and shoots them to survive. This project helped me practice object-oriented programming, collision detection, game loops, and debugging.

## Features

- Spaceship movement and rotation using keyboard controls
- Shooting with a short cooldown between shots
- Asteroids that spawn from random screen edges
- Circle-based collision detection between the player, shots, and asteroids
- Larger asteroids splitting into smaller asteroids when shot
- Game ends when an asteroid collides with the player

## Tech stack

- Python 3.13
- Pygame 2.6.1
- `uv` for environment and dependency management

## Getting started

You will need [uv](https://docs.astral.sh/uv/getting-started/installation/) installed and a desktop environment capable of opening a Pygame window. The repository includes `.python-version`, `pyproject.toml`, and `uv.lock` to define the Python version and dependencies.

1. Clone the repository:

   ```bash
   git clone https://github.com/weaverbtw/asteroids.git
   cd asteroids
   ```

2. Install the project dependencies:

   ```bash
   uv sync
   ```

3. Start the game:

   ```bash
   uv run python main.py
   ```

## Controls

| Key | Action |
| --- | --- |
| `W` | Move forward |
| `S` | Move backward |
| `A` | Rotate left |
| `D` | Rotate right |
| `Space` | Shoot |

Close the game window to quit. The game also ends when your ship collides with an asteroid.

## Project structure

```text
asteroids/
├── main.py           # Main game loop and collision handling
├── player.py         # Player movement, rotation, and shooting
├── asteroid.py       # Asteroid movement and splitting
├── asteroidfield.py  # Asteroid spawning
├── shot.py           # Projectile behavior
├── circleshape.py    # Shared base class and collision checks
├── constants.py      # Game settings
├── logger.py         # Gameplay state and event logging
├── pyproject.toml    # Project metadata and dependencies
├── uv.lock           # Locked dependencies
└── .python-version   # Preferred Python version
```

## What I learned

This was a project I made for Boot.dev. I wrote the gameplay implementation while following the course requirements; some of the more advanced physics-related logic was provided by the course. The project gave me hands-on practice with:

- Designing classes and using inheritance to share behavior
- Updating and drawing game objects with Pygame sprite groups
- Managing movement and collision behavior in a game loop
- Debugging code and using Git for version control

## Current limitations

This version does not include scoring, multiple lives, or a start/restart menu yet.
