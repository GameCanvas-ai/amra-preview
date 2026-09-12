# Tanzane — shipwright shore

The hull is original lofted Blender geometry: curved individual strakes, transverse frames, keel, shaped end planks, sheer rails, treenails and an exposed repair bay. Grounded cradles, slipway, landing, shore ramp, sail work platform, tensioned shade, stitched sail, rope coils, tools and coastal plants are authored geometry. No stock village or boat kit and no concept-image projection are used.

Dry shore sand uses Poly Haven's CC0 `sand_01` by Rob Tuytel, preserved in `../../biomes/CREDITS.md` and `sources.json`. Palm bark reuses the credited CC0 forest material in `../../forest/CREDITS.md`. Hull wood, canvas, rope and water use original procedural materials. The common bake script also packs existing credited scene materials; these are not all visible in this scene.

Lore: `docs/lore/8_gazetteer/alkebu.md:666–682`. Shipyards, repair shops, shipwright and sailmaker guilds, maritime trade and the Tanzane Watchers are established. The southwest coast anchor uses the map's Port Tazane label; public spelling follows the gazetteer. Vessel design, yard layout, plants, tide and sand color are local proposals. This is a shore exploration exterior, not functioning sailing, trading, crafting or a complete port.

Editable source: `browser/docs/art/tanzane.blend`; authoring: `browser/scripts/render-tanzane.py`. Reproduce with `AMRA_BIOME=tanzane blender -b --factory-startup -t 8 --python scripts/render-tanzane.py`, then `python3 scripts/prepare-ataluk.py tanzane`. Close geometry views use `blender -b docs/art/tanzane.blend --python scripts/review-tanzane.py`.
