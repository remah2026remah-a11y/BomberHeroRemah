# BomberHeroRemah Upgrade Plan

## Completed risk slices
- Fixed the runtime crash in powerup animation caused by an out-of-scope `now` variable.
- Prevented level rebuild leaks by disposing the previous ground mesh and resetting the player correctly.
- Reworked explosion presentation into bright cross-shaped flame bursts with particles, screen flash, and decaying camera shake.
- Added continuous hero idle/walk animation, enemy squash-and-stretch, aura rings, bomb glow, and mobile-friendly visual feedback.

## Verification criteria
- JavaScript passes `node --check`.
- Game loads in Chromium without a startup exception.
- Start, movement, bomb placement, explosion, pause, restart, and powerup paths remain wired.
- Rebuilding a stage does not accumulate ground meshes or duplicate player meshes.
