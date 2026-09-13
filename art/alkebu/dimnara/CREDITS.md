# Dimnara — smithy court

The court and equipment are original Blender geometry: a hollow clay furnace with a curved mouth, folded leather bellows and connected nozzle, anvil, tools, cooling vessel, weapon blanks and rack, woven shade, thick plaster walls, recessed wooden doors/windows, terrace supports and drainage, rounded ancillary room and individually modeled thatch reeds. Continuous terrain and irregular repaired paving support the playable route. No stock building kit or projected concept image forms the environment.

Surface textures reuse the credited Poly Haven CC0 plaster, mud and timber in `../../castela/CREDITS.md` and rock/bark in `../../forest/CREDITS.md`. Iron, leather, fired clay, thatch, cloth and ground-wear treatment are procedural. The common helper packs some unused credited materials as well.

Dimnara's weapons/armor economy, craft guilds, Supreme Smith and border trade with Tel'Donor come from `docs/lore/8_gazetteer/alkebu.md:527–545`. This court, equipment technology and regional building treatment are local design proposals. The scene provides exploration and recorded observations; it does not implement crafting recipes, trading, the wider town or multiplayer activity.

Editable source: `browser/docs/art/dimnara.blend`. Reproduce from `browser` with `AMRA_BIOME=dimnara blender -b --factory-startup -t 8 --python scripts/render-dimnara.py`, then `python3 scripts/prepare-ataluk.py dimnara`. Close review: `blender -b docs/art/dimnara.blend --python scripts/review-dimnara.py`; its compositor is disconnected and production-pass hashes are checked for preservation.

## Initial anvil study

The anvil is original Blender geometry: lofted forged body, tapered horn joined into the shoulder, hardened working face and an open square tool socket. Iron materials are procedural. The studio ground is a neutral review surface, not a game environment. The saved source may pack unused credited materials imported by the common scene helper.

The original studio study is a local art proposal for Dimnara's established weapons/armor craft economy (`docs/lore/8_gazetteer/alkebu.md:527–545`). Its specific tool design is not a named canonical artifact. This standalone study preceded the court above and remains an asset inspection view.

Source: `browser/scripts/smithy_anvil.py`, `render-smithy-assets.py`, and `browser/docs/art/dimnara-anvil.blend`. Reproduce from `browser`: `AMRA_BIOME=dimnara blender -b --factory-startup -t 8 --python scripts/render-smithy-assets.py`.
