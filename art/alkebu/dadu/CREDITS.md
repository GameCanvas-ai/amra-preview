# Dadu — winding market lane

The buildings, thick rounded wall shells, terrace construction, openings and fitted doors/windows, recessed work bay and sewn pouches, earthen vault, rooftop reed shade, market awning, laced hide frame, workbench, leather straps, layered textile rolls, hanging cloth and open woven spice baskets are original authored Blender geometry. A bent palm with individually feathered fronds marks the oasis margin; its species and position are local proposals. Continuous terrain and scene obstacles are exported with the render. No projected concept image or stock village kit forms the scene.

Surface materials reuse Poly Haven's CC0 sand (`sand_01`, Rob Tuytel) credited in `../../biomes/CREDITS.md`, plaster and timber credited in `../../castela/CREDITS.md`, and rock/bark credited in `../../forest/CREDITS.md`. Leather, cloth, wicker and spices use procedural materials. The common scene helper may pack unused credited material images as well.

Lore: `docs/lore/8_gazetteer/alkebu.md:343–365`. Dadu's desert trade, stone/adobe architecture, narrow streets, weekly market, leather goods and tribal/family organizations are established. The lane, buildings and goods are local proposals. The original map places Dadu beside the southern Bay of Flames shore, while the text describes a dune-surrounded oasis; this local street does not invent a port or resolve precise shore/dune geography. The sand is not identified as the separate magical Red Sands.

This is an exploration lane with recorded observations. Shops, trading, a scheduled weekly market and the wider city are not implemented by the market props.

Source: `browser/docs/art/dadu.blend` and `browser/scripts/render-dadu.py`. From `browser`, reproduce with `AMRA_BIOME=dadu blender -b --factory-startup -t 8 --python scripts/render-dadu.py`, then `python3 scripts/prepare-ataluk.py dadu`. Close geometry views: `blender -b docs/art/dadu.blend --python scripts/review-dadu.py`. The review script disables/disconnects compositing and verifies production-pass hashes remain unchanged.
