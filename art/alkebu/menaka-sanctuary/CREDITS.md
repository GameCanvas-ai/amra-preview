# Menaka public learning court — local work in progress

Original Blender geometry authored in `browser/scripts/render-menaka-sanctuary.py`: circular earthen sanctuary wall with a doorway, thick domed roof and collar, splayed buttresses, fitted wooden doors and hardware, supported woven reed archive roofs, scroll racks, continuous curved teaching bench, irregular paving, recessed water channel, feathered palms and wheel-formed pottery. This is a proposed threshold and public court, not the complete Great Temple of the Four Winds.

Book, scroll and reading-table construction reuses the original `ivory_library_assets.py` components. The Menaka scene does not reuse Ivory Citadel marble/crystal architecture. No photograph of a building, bookcase or plant is projected onto a stand-in box.

Existing CC0 timber and bark textures retain the credits in `../../castela/CREDITS.md` and `../../forest/CREDITS.md`. Dry-ground texture retains the credits in `../../biomes/CREDITS.md`. Plaster, paving, reeds, water and pottery are procedural materials. Shared authoring imports may pack additional already-credited images. Live character assets retain `../../CREDITS.md` provenance.

Primary lore: repository `docs/lore/8_gazetteer/alkebu.md:634–664`. The architecture, tutor, archive entries and learning task are original local proposals. The garden passage does not assert a surveyed temple position or an exact geographic distance. No copied sacred symbols, named remedies or hidden artifact powers are introduced.

Reproduce from `browser`: `AMRA_BIOME=menaka-sanctuary blender -b --factory-startup -t 8 --python scripts/render-menaka-sanctuary.py`, followed by `python3 scripts/prepare-ataluk.py menaka-sanctuary` and `npm run build:pages`. Editable scene: `browser/docs/art/menaka-sanctuary.blend`.
