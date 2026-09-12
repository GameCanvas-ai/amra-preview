# Ishanlar Wood surface materials

Original 1K color, OpenGL normal and roughness textures from [Poly Haven](https://polyhaven.com), freely available under [CC0 1.0](https://polyhaven.com/license). Downloaded 13 September 2026.

- [Forest Leaves 02](https://polyhaven.com/a/forest_leaves_02) — Rob Tuytel. Used for floor.
- [Bark Brown 02](https://polyhaven.com/a/bark_brown_02) — Rob Tuytel. Used for bark.
- [Rock Face](https://polyhaven.com/a/rock_face) — Greg Zaal, Dario Barresi. Used for rock.

The downloaded images are bundled unchanged. Amra applies tiling, scene tint and lighting. See `sources.json` for source URLs, sizes and MD5 checksums. Reproduce imports with `python3 scripts/import-forest-materials.py`. The importer is powered by Poly Haven’s public API; the game serves bundled local files and makes no live API calls.

The woodland also reuses the CC0 soil and timber materials credited in [../castela/CREDITS.md](../castela/CREDITS.md), and Quaternius leaf/plaster textures credited in [../CREDITS.md](../CREDITS.md). Tree geometry, ground paths, undergrowth arrangement, water shader, clearing composition and canopy fading were authored for Amra.
