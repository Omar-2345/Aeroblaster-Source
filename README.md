# Aeroblaster

A fast-paced 2D platformer shooter built with Python and Pygame. Originally created by DaFluffyPotato, modified and expanded by Omar-2345.

## How to Play

- **A / D** — move left / right
- **W / Space** — jump (double jump supported, second jump gives a higher boost)
- **Mouse** — aim
- **Left Click** — shoot
- Destroy all cores on each level to advance
- Avoid turret shots or you die and restart the level

## Features

### Original
- 7 hand-crafted levels
- Turret enemies that predict your movement
- Particle effects and dynamic camera
- Custom pixel font renderer
- Smooth delta-time based physics

### Added by Omar-2345
- **Live score system** — earn 100 points per core destroyed
- **Combo multiplier** — destroy cores quickly to multiply your score
- **Death counter** — tracks how many times you've died
- **Persistent high score** — saved to `highscore.txt`, loads on startup
- **Double jump boost** — second jump launches you higher
- **Death flash effect** — screen flashes when you die
- **"YOU DIED" screen** — displayed on death before restart
- **HUD** — score, deaths, best score, and combo all shown in top left

## Setup

```bash
pip3 install pygame
python3 Aeroblaster.py
```

## Project Structure

```
Aeroblaster.py       # Main game loop
highscore.txt        # Auto-generated, stores your best score
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

## Credits

Original game by [DaFluffyPotato](https://dafluffypotato.com). Modified and expanded by Omar-2345.
