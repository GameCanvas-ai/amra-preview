# Kupa — local fortress street and roof study

The local scene is original Blender geometry: a continuous hill and bent paved incline, stone houses with fitted clay roofs, retaining walls, round watchtowers, an arched closed gate, shaped brewing vessels, woven grain basket and supported malt-drying rack. The rocky outcrops use modeled erosion and bedding; shrubs and dry grass are authored geometry. This remains a work in progress, not a complete city or final art approval.

Materials reuse the Poly Haven CC0 mud, cobbles and wood credited in `../../castela/CREDITS.md`, and rock/bark credited in `../../forest/CREDITS.md`. Clay, plant, grain and fiber materials are procedural. Original source: `browser/scripts/render-kupa.py`, `kupa_roof.py`, `review-kupa.py` and `browser/docs/art/kupa.blend`.

From `browser`: `AMRA_BIOME=kupa blender -b --factory-startup -t 8 --python scripts/render-kupa.py`, then `python3 scripts/prepare-ataluk.py kupa`. The color, depth and motion passes share the authored camera. Terrain and collision export from the same height function. Close construction reviews disconnect compositing and verify that production pass hashes remain unchanged.

The hill, fortifications, stone/red-tile architecture and beer trade follow `docs/lore/8_gazetteer/alkebu.md:597–615`; the street arrangement, brewing equipment and three-metre local ascent are design proposals. No gate interior, brewing recipe, trade simulation or complete city is implemented.

## Retained roof construction study

This is an original geometry study of overlapping red clay pan tiles, curved joint covers and ridge caps, supported by timber rafters and battens. Exposed edges show actual clay thickness and open curved profiles. Clay materials are procedural; timber reuses the Poly Haven CC0 material credited in `../../castela/CREDITS.md`. The shared helper may pack unused credited images too.

Kupa's stone buildings and red-tile roofs are explicit in `docs/lore/8_gazetteer/alkebu.md:597–615`. This tile arrangement, roof pitch and joinery are local design proposals. The neutral floor and four temporary supports are studio review equipment, not a Kupa building or scene.

Source: `browser/scripts/kupa_roof.py`, `render-kupa-roof.py` and `browser/docs/art/kupa-roof.blend`. Reproduce from `browser` with `AMRA_BIOME=kupa blender -b --factory-startup -t 8 --python scripts/render-kupa-roof.py`. The script exports `roof-review.png` and `roof-underside-review.png`; it does not create playable terrain, scenery/depth passes or a Kupa journey entry. The floor is hidden from the underside camera to avoid clipping the orthographic inspection view.
