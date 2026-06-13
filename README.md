# Aeroblaster

A fast-paced 2D platformer shooter built with Python and Pygame.

## How to Play

- **A / D** — move left / right
- **W / Space** — jump (double jump supported)
- **Mouse** — aim
- **Left Click** — shoot
- Destroy all cores on each level to advance
- Avoid turret shots or you die and restart the level

## Features

- 7 hand-crafted levels
- Turret enemies that predict your movement
- Particle effects and dynamic camera
- Live score, death counter, and persistent high score
- Double jump boost mechanic

## Setup

```bash
pip3 install pygame
python3 Aeroblaster.py
```

## Project Structure

```
Aeroblaster.py       # Main game loop
data/
  engine.py          # Entity, animation, particle system
  tileset_loader.py  # Loads tile images
  text.py            # Custom pixel font renderer
  outline.py         # Sprite outline effect
  fps.py             # Frame rate tracking
  levels/            # Level data (JSON tile maps)
  images/            # Sprites, tiles, fonts
  sfx/               # Sound effects
  music.wav          # Background music
```
