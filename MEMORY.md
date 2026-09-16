# Development Notes

The original repository contained only `index.html`. The most important runtime defect was `updatePowerups()` referencing `now`, which only existed as a local variable in `animate()`. Level rebuilding also left the previous ground plane in the scene, and starting a fresh game detached the player reference without removing its mesh. These are now corrected.
