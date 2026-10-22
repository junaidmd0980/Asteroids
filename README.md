# Asteroids

A classic Asteroids-inspired arcade game built with Python and Pygame.

## 🚀 Features

- **Player Ship:** Smooth movement and rotation mechanics.
- **Combat:** Ability to shoot projectiles at incoming targets.
- **Dynamic Elements:** Randomly spawning asteroids to clear.
- **Engine Architecture:** Sprite-based update and rendering system.
- **Collisions:** Circle-based game objects configured and ready for collision detection.

## 📋 Requirements

- **Python 3.13** or newer
- [uv](https://docs.astral.sh/uv/) (recommended for package management)

## 🛠️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/junaidmd0980/Asteroids.git
   cd Asteroids
   ```

2. **Install dependencies** and automatically create the virtual environment:
   ```bash
   uv sync
   ```

3. **Run the game:**
   ```bash
   uv run python main.py
   ```

## 🎮 Controls

| Key | Action |
| :--- | :--- |
| **W** | Move forward |
| **A** | Rotate left |
| **D** | Rotate right |
| **Space** | Shoot projectile |
| **Close Window** | Quit the game |

## 📁 Project Structure

```text
Asteroids/
├── main.py          # Application entry point and main game loop
├── constants.py     # Screen, player, asteroid, and gameplay constants
├── circleshape.py   # Shared base class for circular sprites
├── player.py        # Player ship movement and shooting
├── shot.py          # Projectile behavior
├── asteroid.py      # Asteroid behavior
├── asteroidfield.py # Asteroid spawning logic
├── logger.py        # Game-state logging utilities
├── pyproject.toml   # Project metadata and dependencies
├── uv.lock          # Locked dependency versions
└── README.md        # Project documentation
```

## 📝 Development Notes

- **Pygame:** Used extensively for rendering, user input, timing, vector physics, and managing sprite groups.
- **uv:** Handles rapid dependency and isolated virtual environment management.
- **Collisions:** Utilizes custom circle-based collision helpers inherited from `CircleShape`.
- **Git Hygiene:** Local runtime environment files (like `.venv/`) and generated tracking logs (`game_state.jsonl`, `game_events.jsonl`) should **not** be committed to the repository.

## 🎓 Learning Project

This project was built as a capstone experience while following the **Boot.dev** Python and Pygame curriculum. 👍
