# Red Sands playable scene

Authored Blender geometry and terrain for Amra. No generated illustration is projected onto the scene.

Ground uses the previously imported Poly Haven `red_sand` CC0 material; ruined masonry uses the credited forest rock surface. See `../../biomes/CREDITS.md`, `../../biomes/sources.json`, `../../forest/CREDITS.md` and `../../forest/sources.json` where present for the original imports. Procedural wind forms, chipped masonry and scene layout are project art.

Primary lore: Amra Alkebu gazetteer, Red Sand Desert, lines 700–710. The magical red sands and forgotten ruins are established; this unnamed threshold, its construction and its exact position are proposals. No deity or living-clan insignia is assigned. No ordinary oasis vegetation is included.

Reproduction: `AMRA_BIOME=red-sands blender -b --factory-startup -t 8 --python scripts/render-alkebu.py`, then `python3 scripts/prepare-ataluk.py red-sands`, from the private source repository's `browser` directory.
