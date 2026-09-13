# Torum Keep modeled lodging study

Original Blender geometry authored for Amra. The communal hearth refinement in scripts/dhon_hearth.py adds constructed arch stones, chimney, pantry joinery, barrel staves, herbs, cookware, draped cloth and a procedural woven carpet; these are all geometry or surface materials in the shared scene. The approved dwelling concept D guides the domestic layout, warm light and carved stone; it is not projected onto scenery. Color and 16-bit depth are rendered together from the saved scene. Terrain clearance is sampled from evaluated wall, doorway and furniture meshes.

Shared CC0 surface materials: Poly Haven Rock Face (Greg Zaal, Dario Barresi), credited in ../../forest/CREDITS.md, and wood credited in ../../castela/CREDITS.md. Textiles, ceramic and metal use authored procedural materials. No architectural photograph or generated scene is used as a material.

Gazetteer: docs/lore/8_gazetteer/dhon_toruhm.md, Torum Keep, lines 466–476. The lodging layout is an original interpretation; it is not a canonical surveyed floor plan.

Reproduce from repository root:
AMRA_REGION=dhon-toruhm AMRA_BIOME=keep-dwellings-geometry ATALUK_SAMPLES=96 /opt/homebrew/bin/blender -b --factory-startup -t 8 --python browser/scripts/render-dhon-dwellings.py
AMRA_REGION=dhon-toruhm python3 browser/scripts/prepare-ataluk.py keep-dwellings-geometry

Status: playable geometry study. Further surface wear, architectural variety, mountain integration and character art refinement remain. The four other Dhon scenes currently retain the experimental painted pipeline.
