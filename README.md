# Cluck & Load 🐔🔫

A browser-based **Moorhuhn-style shooting gallery** — 90 seconds to rack up as
many points as you can plucking birds out of the sky.

**▶️ Play it: https://github.freaxnx01.ch/game-cluck-and-load/**

## How to Play

| Action | Control |
| --- | --- |
| **Fire (shotgun)** | Click — 6-shell magazine, `R` to reload |
| **Fire (machine gun)** | Hold left mouse — 50-round belt, watch the heat bar |
| **Fire (sniper)** | Click — 5 rounds, scope overlay with mildots |
| **Fire (missile)** | Click — 3 homing missiles, auto-locks nearest target |
| **Cycle weapon** | `M` (shotgun → machine gun → sniper → missile → shotgun) |
| **Start / restart** | Click on the menu or game-over screen |

Game always starts with the shotgun. Press `M` mid-game to cycle through all four weapons.

## Game Content

**Birds:**
- **Normal** (10 pts) — standard flock
- **Fast** (25 pts) — smaller, quicker, worth more per grey feather
- **Golden** (50 pts) — rare, sparkling, high value
- **Big** (15 pts) — slow, oversized target
- **Pop-up chicken** (30 pts) — pops head from below, close to camera, bonus points

**Special targets:**
- **UFO** (100 pts) — rare flying saucer with blinking lights and beam; big explosion + sound when hit

**Weapons:**
- *Shotgun* — 6 shells, combo multiplier up to x5 for consecutive hits, high damage per shot
- *Machine gun* — 50-round belt, sustained fire with a heat bar (overheats on sustained spray), no combo bonus
- *Sniper rifle* — 5 rounds, scope overlay with vignette and mildots, +50 bonus pts per kill, slow reload
- *Missile* — 3 homing missiles that lock onto nearest target (birds, UFOs, pop-ups), big explosion on impact

**Environment:**
- Dynamic time-of-day: sky transitions from dawn → noon → sunset over the 90-second round
- Weather: rain storms with darkening sky, raindrops, and a rainbow that appears as rain clears
- Procedural parallax background (sky, sun, clouds, mountains, hills, trees, grass)

**Feedback:** score/combo HUD, best-combo and accuracy tracking, final stats
screen (birds hit / total, accuracy %, best combo, shots fired, weapon used),
synthesized Web Audio sounds (shot, MG, sniper, missile launch, lock, hit, reload,
overheat, explosion), particle effects (feathers, muzzle flash, shell casings,
sparks, missile trails, smoke).

## Tech Stack

- Single self-contained `index.html` — no build step, no dependencies, no
  image/audio assets. Canvas 2D for rendering, Web Audio API (synthesized) for
  sound.
- Procedural parallax background with time-of-day color interpolation, weather
  system, and hand-drawn vector bird/UFO/missile sprites.

## Running Locally

No build needed — just open `index.html` in a browser.

## Credits

Built by [Claude](https://claude.com/claude-code).
