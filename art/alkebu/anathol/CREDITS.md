# Anathol construction assets — work in progress

Original Blender-authored geometry: a thick white-marble architectural bay, fitted arch stones and timber door, continuous interlaced relief, door-panel carving and metal fittings; an eight-panel curved lantern with ribs, vented crown, bail pivots, linked suspension and wall bracket; and a timber textile stall with lashings, draped shade, framed counter, spirally wound cloth bolts and hanging samples.

These are local design proposals grounded in the white-marble capital and colorful Thousand Lights Market in `docs/lore/8_gazetteer/alkebu.md:301–323,726–736,748–758`. The carvings are original geometric motifs, not canonical clan emblems or copied sacred symbols. No complete Anathol environment, functional store, council interior or region is claimed.

Marble, bronze, diffuser and fabric materials are procedural. Timber uses the Poly Haven CC0 wood material already credited in `../../castela/CREDITS.md`. The shared authoring helper may pack additional existing credited images even when this study does not use them.

Editable source: `browser/scripts/anathol_architecture.py`, `render-anathol-study.py`, `review-anathol-night.py` and `browser/docs/art/anathol-study.blend`. From `browser`, reproduce with `AMRA_BIOME=anathol blender -b --factory-startup -t 8 --python scripts/render-anathol-study.py`.

Review PNGs are isolated construction views. The neutral floor is studio equipment, not game terrain. Compositing is disconnected and no scenery, depth, motion or walkable-grid passes are exported by this study. A future full scene must generate and verify those together.

## Local market passage under development

`render-anathol.py` and `docs/art/anathol.blend` assemble an original paved passage, enclosed market house, shuttered windows, textile and jewelry counters, and supported lantern posts. Paving also uses the CC0 rock material credited in `../../forest/CREDITS.md`; other existing material credits above apply. The closed building, individual layout and merchandise arrangements are proposals, not a complete capital or implemented trade system.

The full-scene authoring script exports aligned color/depth/motion passes, terrain and obstacles; `prepare-ataluk.py anathol` creates the runtime JPEG and packed depth. Optional dusk/lamp metadata accompanies the bake so the live actor can use regional lighting. This passage remains a work in progress. The separately published construction-review images are not proof of gameplay completion.

The passage also includes original curved spice-vault masonry, reed baskets, spice heaps and expanded street paving. A separately baked canopy cutaway preserves nearby character visibility. Three idle residents use the existing character assets credited in `../../CREDITS.md`; their anonymous roles and placements are local proposals. No dialogue, buying, crafting or quests are implied.
