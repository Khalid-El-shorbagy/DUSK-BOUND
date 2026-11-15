# Moss swordsman (SpriteCanvas character pack)

Moss swordsman exported from SpriteCanvas as a Godot 4 character pack, facing both ways. Released CC0 (public domain): use it in any project.

- `character.json` lists the 14 animations (`idle`, `run`, `jump`, `attack`, `skill`, `hurt`, `death`, each `_east` and `_west`) with frame counts, loop flags and file paths.
- `godot/character.tscn` is an `AnimatedSprite2D` with every animation. The frame pivot (the feet) sits on the node origin, so place the node where the character should stand.
- `godot/character.tres` is the `SpriteFrames` resource on its own.
- `animations/<name>/atlas.png` is the sprite atlas, `animations/<name>/export.json` holds frame timing, atlas rectangles, trim offset and pivot.

Keep `godot/` and `animations/` side by side: the SpriteFrames reference the atlases by relative path.

The west animations are horizontal mirrors of the east ones, with the pivot mirrored too.

This copy is trimmed: private ids are replaced with `"swordsman"`, and the per-frame PNGs, receipts and manifests are left out (the `frames/` paths inside `export.json` are informational only).

Made with SpriteCanvas: https://spritecanvas.com/free-sprite-sheets/
