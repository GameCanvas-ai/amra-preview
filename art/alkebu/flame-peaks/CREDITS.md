# Flame Peaks — Sacred Fire exterior

The guardian sculptures begin with Quaternius CC0 male and female anatomical meshes from the imported Standard character pack. The original license is preserved at `../../characters/LICENSE.txt`, with upstream attribution in `../../CREDITS.md`. The posed sculptures are modified assets: frozen distinct poses, fitted carved garments and head coverings, collars, wrist cuffs, pleated wraps, convex solar shields, spears and material treatment authored for this scene. They are not unchanged player-character instances.

Sanctuary masses, cut masonry joints, concave cornices, portal, relief details, doors, plinths, paving, terrain and layout are authored Blender geometry. Rock and wood textures reuse the credited CC0 imports in `../../forest/CREDITS.md` and `../../castela/CREDITS.md`. Other surfaces are procedural materials. No concept image is projected as scenery.

Primary lore: Alkebu gazetteer, Temple of the Sacred Fire, lines 760–772; Burning Sun Clan, lines 84–99; religions reference, Ethoras and Necis. Red stone, red/gold detail, and two colossal warriors bearing spears and shields are established. Their specific poses, clothing, facial features and local architectural forms are proposals. The figures do not assert named historical identities. This is an exterior; the altar flame, interior and priest interactions are not implemented.

Private source: `browser/scripts/flame_guardians.py`, `render-flame-guardians.py`, `render-flame-peaks.py`, and packed `browser/docs/art/flame-guardians.blend` / `flame-peaks.blend`.

Reproduce from `browser`: `AMRA_BIOME=flame-peaks blender -b --factory-startup -t 8 --python scripts/render-flame-peaks.py`, then `python3 scripts/prepare-ataluk.py flame-peaks`. The guardian studio review uses `render-flame-guardians.py` with the same environment variable.
