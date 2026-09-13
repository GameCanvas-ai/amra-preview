# White Ice Mountains — initial local fortress study

Original scene geometry in `browser/scripts/render-white-ice.py`: continuous rock and snow terrain, interpolated snow coverage, compacted approach, fitted angular stone portal and relief, separate iron gate plates/straps/rivets/pulls, terrain-following ice sheet, tapered icicles, structural snow cover and forged braziers with individual glowing coals. No external scene image or franchise game asset is projected onto this geometry.

Rock, cut stone, snow, ice, iron and embers use original procedural materials. Shared authoring helpers can pack existing CC0 textures without applying them to this scene; their attribution remains in the existing Castela/forest credits. Live dwarf characters use the existing licensed character kit credited in `../../CREDITS.md`.

Lore: `docs/lore/8_gazetteer/dhon_toruhm.md:562–570`, with original map review in `DHON_TORUHM_PRODUCTION.md`. This is an unnamed local fortress approach. Geometry, relief designs, braziers and anonymous dwarf residents are proposals. It is not Torum Keep, Erebor Fortress or the lost city of giants. Avalanche/blizzard hazards and fortress interiors are not implemented.

Reproduce from `browser`: `AMRA_REGION=dhon-toruhm AMRA_BIOME=white-ice blender -b --factory-startup -t 8 --python scripts/render-white-ice.py`, then `AMRA_REGION=dhon-toruhm python3 scripts/prepare-ataluk.py white-ice`. Editable scene: `browser/docs/art/white-ice.blend`. This initial study still needs architectural and environmental art refinement.
