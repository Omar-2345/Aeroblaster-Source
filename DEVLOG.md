# Aeroblaster — Dev Log

A personal record of changes and additions made to the original Aeroblaster source code.

---

## June 2026 — Project Start

**What I started with:**
- Downloaded the original Aeroblaster pygame source
- A complete 7-level platformer shooter with tile maps, physics, turrets, particles, and a custom pixel font
- Single file main game loop (`Aeroblaster.py`) with helper modules in `data/`

---

## Changes Made

### Score System
- Added a `score` variable starting at 0
- Each core destroyed awards **100 points**
- Score displayed live on the HUD (top left)

### Death Counter
- Added a `deaths` variable to track how many times the player has died
- Displayed on HUD alongside score

### High Score (Persistent)
- High score saved to `highscore.txt` on disk
- Automatically loads on startup and updates whenever a new best is reached
- Displayed on HUD as "best: X"

### Double Jump Boost
- Second jump now launches the player slightly higher (`-6` gravity instead of `-5`)
- Makes movement feel snappier and more rewarding

### Death Flash Effect
- Added extra flash particles on player death for visual impact

---

## What I Want to Add Next

- [ ] A proper main menu screen
- [ ] Sound toggle (mute button)
- [ ] Timer-based bonus score for fast level completion
- [ ] Player health bar instead of instant death
- [ ] More levels

---

## What I Learned

- How a tile-map based level system works in pygame
- How delta time (`dt`) keeps game speed consistent across different machines
- How to use particle systems for visual effects
- How pygame's sprite and surface system works
