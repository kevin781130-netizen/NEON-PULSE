# NEON PULSE — Synesthetic Evolution

This branch evolves only the audiovisual presentation layer. The existing gameplay core and the user's music assets remain intact.

## Preserved
- LEVEL / SURVIVAL / SPRINT rules and timing
- Board dimensions, movement, rotation, hold, ghost piece and hard drop
- T-Spin, combo, back-to-back, score and level progression
- `menu.mp3`, `level.mp3`, `survival.mp3`, `sprint.mp3`
- Existing BGM volume: 0.24

## Added
- Music-spectrum-driven fullscreen particles and orbital light
- Different visual palettes for each existing mode
- Visual bursts on hard drop, line clear, T-Spin, level-up and perfect clear
- Board bloom, impact ring and upgraded block surface treatment
- Reduced-motion fallback
- Lower particle count on mobile

## Architecture
The effect engine is isolated in `effects.js` and `effects.css`. `index.html` only exposes a few visual hooks, so the game logic remains easy to audit and revert.

The design direction is inspired by the audiovisual synchronization philosophy of *Tetris Effect: Connected* without copying its assets or gameplay systems.
