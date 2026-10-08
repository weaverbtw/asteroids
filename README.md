# Asteroids

A small arcade-style Asteroids game built in Python using Pygame.

## Overview

This project is a classic Asteroids-inspired game where the player controls a spaceship, avoids incoming asteroids, and shoots them down to survive as long as possible. The game includes movement, shooting, and simple gameplay loops typical of the arcade classic.

## Features

- Player ship movement and rotation
- Bullet firing
- Asteroid spawning and collision detection
- Simple, lightweight Pygame-based setup

## Requirements

To run this project, you need:

- Python 3.10 or newer
- Pygame 2.x
- A desktop environment with a display (for local gameplay)

Optional:

- Virtual environment tooling such as venv
- Git for version control

## Installation

1. Open a terminal in the project folder.
2. Create and activate a virtual environment:

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Install the required dependency:

   ```bash
   pip install pygame
   ```

## Running the Game

From the project root, start the game with:

```bash
python main.py
```

If your entry point is named differently, use that file instead (for example `python src/main.py` or similar).

## Controls

- Move: W/A/S/D or arrow keys
- Fire: Space
- Quit: ctrl + c in terminal


## Notes

- The project is designed for local desktop play.
- If you want to add sound effects, sprites, or a menu screen, those can be added in the game module files.
- Make sure your Python environment is active before running the project.

## License

This project is provided for educational and personal use. Add a license if you want to share it publicly under specific terms.
