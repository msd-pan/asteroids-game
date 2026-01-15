# Asteroids Game

A classic arcade-style asteroids game built with Python and Pygame. Control a spaceship, shoot asteroids, and survive as long as you can!

## Features

- Classic asteroids gameplay mechanics
- Smooth player movement and rotation controls
- Shooting system with cooldown mechanics
- Asteroid splitting - larger asteroids break into smaller, faster ones when destroyed
- Collision detection between player, asteroids, and shots
- Procedural asteroid spawning system
- Game state and event logging for analytics

## Requirements

- Python >= 3.12
- Pygame 2.6.1

## Installation

### Option 1: Using uv (Recommended)

This project uses [uv](https://github.com/astral-sh/uv) for dependency management.

1. Clone the repository:
```bash
git clone <your-repo-url>
cd asteroids-game
```

2. Install uv if you haven't already:
```bash
pip install uv
```

3. Install dependencies:
```bash
uv sync
```

4. Run the game:
```bash
uv run python main.py
```

### Option 2: Using pip and venv

1. Clone the repository:
```bash
git clone <your-repo-url>
cd asteroids-game
```

2. Create a virtual environment:
```bash
python -m venv .venv
```

3. Activate the virtual environment:
   - On Linux/Mac:
     ```bash
     source .venv/bin/activate
     ```
   - On Windows:
     ```bash
     .venv\Scripts\activate
     ```

4. Install dependencies:
```bash
pip install pygame==2.6.1
```

5. Run the game:
```bash
python main.py
```

## How to Play

- **Arrow Keys / WASD**: Rotate and move the spaceship
  - Up/W: Move forward
  - Left/A: Rotate left
  - Right/D: Rotate right
- **Spacebar**: Shoot
- **Goal**: Destroy asteroids and avoid collisions

The game ends when your spaceship collides with an asteroid. Try to survive as long as possible!

## Game Configuration

You can modify game settings in [constants.py](constants.py):

- Screen resolution (default: 1280x720)
- Player speed and turning rate
- Asteroid spawn rate and sizes
- Shooting cooldown and projectile speed

## Project Structure

- [main.py](main.py) - Main game loop and initialization
- [player.py](player.py) - Player spaceship class and controls
- [asteroid.py](asteroid.py) - Asteroid class and splitting logic
- [shot.py](shot.py) - Projectile class
- [asteroidfield.py](asteroidfield.py) - Asteroid spawning system
- [circleshape.py](circleshape.py) - Base class for circular game objects
- [constants.py](constants.py) - Game configuration constants
- [logger.py](logger.py) - Game state and event logging

## License

This project is built as part of the [Boot.dev](https://boot.dev) curriculum.
