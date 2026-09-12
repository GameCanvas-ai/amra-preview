# Nuzai — mine and craft yard

Terrain, excavated gallery surfaces, geological cut sections, rough portal returns, fitted timber frames, support straps, windlass/wheel/rope, hauling sled, ore-sorting bench, baskets, clay lamps, wall masonry and plants are authored Blender geometry. No flat concept image or dark rectangle is projected onto the mine entrance.

Rock and timber textures reuse the credited CC0 sources in `../../forest/CREDITS.md` and `../../castela/CREDITS.md`. Yard sand uses Poly Haven's CC0 `sand_01` by Rob Tuytel, preserved in `../../biomes/CREDITS.md` and its source manifest. Other materials are original procedural surfaces. Source packing may include unused shared materials; that does not mean every packed texture is visible here.

Source lore: repository `docs/lore/8_gazetteer/alkebu.md:427–443`. Nuzai's mountain-shadow location, gold/silver mine, fortified city and mining/artisan economy are established. The mine entrance, supports, gallery dimensions, tools, lamps and local yard are design proposals. No working mining reward, crafting recipe, shop, deeper dungeon or named ore vein is claimed.

The roof and camera-facing rock have a second view with closed geological cross-sections. Original shadows remain; the cut faces receive restrained fill so their rock texture is readable. These are visual cut surfaces, not additional walkable terrain. Touch selection uses the depth of the surface actually revealed near the character.

Editable source: `browser/docs/art/nuzai.blend`. Reproduce from `browser`: `AMRA_BIOME=nuzai blender -b --factory-startup -t 8 --python scripts/render-nuzai.py`, then `python3 scripts/prepare-ataluk.py nuzai`. `review-nuzai.py` produces close views from the saved source.
