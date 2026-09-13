# Raha vineyard margin — work in progress

Original Blender geometry from `browser/scripts/render-raha-vineyard.py`: gnarled vine stems and roots, trained shoots, lobed folded leaves and veins, grape clusters, stakes and fibre lines, reed baskets and shade, hollow clay jar and fitted boundary stones. Layout and craft construction are local proposals grounded in Raha’s agriculture, vineyards and weaving in `docs/lore/8_gazetteer/alkebu.md:393–425`.

Existing CC0 textures: dry ground credited in `../../biomes/CREDITS.md`; wood credited in `../../castela/CREDITS.md`; bark/stone credited in `../../forest/CREDITS.md`. Procedural leaf, fruit, fibre and clay materials are original. Shared authoring utilities may pack other existing credited textures. Character assets retain `../../CREDITS.md` credits.

The editable full scene is `browser/docs/art/raha-vineyard.blend`; reproduce from browser with `AMRA_BIOME=raha-vineyard blender -b --factory-startup -t 8 --python scripts/render-raha-vineyard.py`, then `python3 scripts/prepare-ataluk.py raha-vineyard`. Color/depth/motion, terrain and shade cutaway must be regenerated together. This vineyard does not implement the full city, trading or harvesting.
