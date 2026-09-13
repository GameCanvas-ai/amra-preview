# Ivory Citadel reading gallery — local work in progress

Original geometry in `ivory_library_assets.py` and `render-ivory-library.py`: framed shelving, shaped posts and supports, bound manuscripts with covers/spines/page groups and binding bands, curved open pages with original decorative pen marks, rolled parchment and cores, joined reading tables, fitted marble construction and faceted crystalline elements. No shelf or book photograph is projected onto a stand-in box. Pen marks are original decorative marks, not copied text or a canonical named tome.

Timber uses the existing CC0 material credited in `../../castela/CREDITS.md`. The dark cutaway surround, marble, leather, parchment, ink, woven mats and crystal materials are procedural; shared authoring helpers may pack other already credited textures. Character models retain `../../CREDITS.md` credits. Marble construction helpers are shared with the original Anathol kit.

`ivory_gallery_architecture.py` adds thick arched clerestory openings, fitted arch surrounds, projecting sills, open forged diamond lattice, profiled wall moldings and carved pilasters. Its geometric interlace is an original local art proposal, not a copied sacred motif. Reading mats are thin shaped meshes with modeled knotted fringe; the windows have actual open apertures. Isolated saved-scene construction review and aperture ray checks are in `review-ivory-gallery.py`.

The gallery layout and furnishings are local proposals grounded in `docs/lore/8_gazetteer/alkebu.md:712–724,172–182`. The crystalline study specimen is explicitly not the hidden Eye of Anaya. Exact exterior geography, the complete library/citadel, scholar dialogue and artifact mechanics remain unimplemented.

Editable full scene: `browser/docs/art/ivory-library.blend`. Reproduce from browser with `AMRA_BIOME=ivory-library blender -b --factory-startup -t 8 --python scripts/render-ivory-library.py`, then `python3 scripts/prepare-ataluk.py ivory-library`. Separate study source: `render-ivory-study.py` and `docs/art/ivory-library-study.blend`; its neutral studio floor is not a game environment.
