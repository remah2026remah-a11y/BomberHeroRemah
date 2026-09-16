# Runtime Structure

The project is a single self-contained Three.js browser game in `index.html`. The file owns UI, procedural meshes, scene construction, game state, input, animation, and rendering. The upgrade keeps this lightweight architecture while adding explicit lifecycle state for the ground mesh, camera shake, game clock, and character animation metadata.
