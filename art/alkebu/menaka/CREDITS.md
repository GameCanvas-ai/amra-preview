# Menaka oasis garden

Authored Blender geometry and terrain for Amra. No generated illustration is projected onto the scene.

Ground, bark and timber reuse the credited Poly Haven CC0 material imports in `../../biomes/CREDITS.md`, `../../forest/CREDITS.md` and `../../castela/CREDITS.md`. Palm fronds, garden plants, earthen court, woven reed shade and the water basin are authored meshes and procedural materials.

Primary lore: Amra Alkebu gazetteer, Menaka, lines 634–652. Oases, gardens, pilgrimage and learning are established. The basin, its intake, palm species and local garden plan are proposals. This is not the Great Temple of the Four Winds and does not invent its iconography. The local palette is intentionally distinct from the magical Red Sands.

Reproduction: `AMRA_BIOME=menaka blender -b --factory-startup -t 8 --python scripts/render-menaka.py`, then `python3 scripts/prepare-ataluk.py menaka`, from the private source repository's `browser` directory.
