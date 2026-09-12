# Jungle of the Fangs — forest-floor passage

Original authored Blender meshes: continuous branched trunks, flared buttress roots, broadleaf crowns, lianas, fern fronds, thorn stems, litter, sedges, decaying timber and eroded masonry. Recipe: `browser/scripts/render-fangs.py`; packed source: `browser/docs/art/fangs.blend` in the private repository.

Ground, bark, stone and exposed timber reuse the Poly Haven CC0 texture imports documented in `../../forest/CREDITS.md` and `../../castela/CREDITS.md`. Remaining surfaces are original procedural materials. No concept illustration or AI-generated plate is used as scenery.

Canon source: `docs/lore/8_gazetteer/alkebu.md`, Jungle of the Fangs, lines 774–784. Black Lion territory, tangled jungle, murky swamps, medicinal plants and hidden ruins are established. Specific trees, plants, trail, local water course and unnamed masonry are design proposals. This exterior does not implement a temple interior, predators, harvestable medicines or a named tribe's settlement.

Camera-visible canopy has a separate object mask. The second color/depth bake hides upper leaves from camera rays while preserving their shadows, allowing a localized gameplay cutaway. Roots, trunks and understory remain visible. Terrain heights and collision use the same source geometry functions as the render.

Reproduction from `browser`: `AMRA_BIOME=fangs blender -b --factory-startup -t 8 --python scripts/render-fangs.py`, then `python3 scripts/prepare-ataluk.py fangs`.
