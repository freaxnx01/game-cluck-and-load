# Cluck & Load 🐔🔫

A browser-based **Moorhuhn-style shooting gallery** — 90 seconds to rack up as
many points as you can plucking birds out of the sky.

**▶️ Play it: https://github.freaxnx01.ch/game-cluck-and-load/**

## How to Play

| Action | Control |
| --- | --- |
| **Fire (shotgun)** | Click — 6-shell magazine, `R` to reload |
| **Fire (machine gun)** | Hold left mouse — 50-round belt, watch the heat bar |
| **Switch weapon** | `M` |
| **Start / restart** | Click on the menu or game-over screen |

## Game Content

**Birds:**
- **Normal** (10 pts) — standard flock
- **Fast** (25 pts) — smaller, quicker, worth more per grey feather
- **Golden** (50 pts) — rare, sparkling, high value
- **Big** (15 pts) — slow, oversized target

**Weapons:**
- *Shotgun* — 6 shells, combo multiplier up to x5 for consecutive hits, high damage per shot
- *Machine gun* — 50-round belt, sustained fire with a heat bar (overheats on sustained spray), no combo bonus

**Feedback:** score/combo HUD, best-combo and accuracy tracking, final stats
screen (birds hit / total, accuracy %, best combo, shots fired, mode used),
synthesized Web Audio sounds (shot, reload, hit, overheat), particle effects
(feathers, muzzle flash, shell casings, sparks).

## Tech Stack

- Single self-contained `index.html` — no build step, no dependencies, no
  image/audio assets. Canvas 2D for rendering, Web Audio API (synthesized) for
  sound.
- Procedural parallax background (sky, sun, clouds, mountains, hills, trees,
  ground) and hand-drawn vector bird sprites.

## Running Locally

No build needed — just open `index.html` in a browser.

## Credits

Built by [Claude](https://claude.com/claude-code).
