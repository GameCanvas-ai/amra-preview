# Dragon Fang river ravine

Original authored Blender landscape and mesh work for Amra: continuous cliff/ledge terrain, displaced embedded rock forms, river surface, uneven falling-water threads, foam, crevice plants and rubble. No generated concept illustration is projected onto the scene.

Rock and ground surfaces reuse the Poly Haven CC0 texture import documented in `../../forest/CREDITS.md`, desaturated for the local rock treatment. Water, foam and plants use original procedural materials. Packed source and reproduction recipe are `browser/docs/art/dragon-fang.blend` and `browser/scripts/render-dragon-fang.py` in the private repository.

Primary lore: `docs/lore/8_gazetteer/alkebu.md`, Dragon Fang Mountains, lines 738–746. Southeastern mountains, clear rivers, cascading waterfalls and nomadic peoples are supported. Specific rock color, plants, local ravine and walking route are proposals. This is not the Flame Peaks, a named tribe's camp or a completed climbing/combat system.

The terrain mesh and navigation grid share the same height function. Horizontal water occupies the red motion mask; falling water occupies green only in scenes with the waterfall metadata flag. Dynamic color movement preserves the baked depth geometry. The river is blocked for this walking demo.

Reproduce from `browser`: `AMRA_BIOME=dragon-fang blender -b --factory-startup -t 8 --python scripts/render-dragon-fang.py`, then `python3 scripts/prepare-ataluk.py dragon-fang`.
