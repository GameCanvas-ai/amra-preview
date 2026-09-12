# Alkebu landscape field notes

Status: implementation reference from lore and map review; scene forms remain proposals. 13 September 2026. Scope is Alkebu only. The accepted gritty isometric rendering language is retained. This document replaces the assumption that one oasis, or one red desert, can stand for the whole region.

## Evidence and source priority

Primary text: repository-root `docs/lore/8_gazetteer/alkebu.md`. Primary visual: `docs/lore/amra_world_map.jpeg`, 4096 × 2048 pixels, north at the top. The review uses a viewport onto this unchanged map with a study anchor overlay. The machine-readable atlas (`world/atlas/places.json`, `world_features.json`, `east_semantic_layers.json`) helps locate named anchors but is derived and contains documented inconsistencies. Its pins are approximate overview positions, not surveyed boundaries, hydrology or placement of the small scene shown.

The shared study record is `browser/client/alkebuRegions.ts`. IDs, source passages, map anchors, direct lore facts, visual proposals, exclusions and water notes are used by the review UI. Full implementation should extend those records rather than creating another disconnected palette list. `art/pipeline/profiles/alkebu.json` is an older derived profile; its single oasis default does not describe all these areas.

## Map reading

- **Northwestern Alkebu:** the Red Sands lie south of the Peaks of the Draken. This red desert is not the whole southern peninsula.
- **Southwest:** Fang Forest is visibly wooded; Menaka and the map's Port Tazane sit farther south/southwest. Their relative placement guides separate ecological treatments, not a claim that Menaka's entire surroundings are dry sand.
- **Anathol/Ataluk belt:** the map shows settlement, water and vegetation around the capital and the plains southwest of it. The gazetteer explicitly makes Ataluk agricultural. Irrigated cultivation must have a local water story.
- **East of Anathol:** Flame Peaks have a distinct map label and a drawn crater. They are separate from the Dragon Fang range in this reference. A crater does not require every approach scene to have flowing lava.
- **Southern/southeastern peninsula:** Dragon Fang Mountains extend toward the Dimnara–Cerenan–Kupa area; forests, slopes and drainage break up the terrain.
- **Southwest coast:** Port Tazane/Tanzane provides a supported maritime anchor. Jungles of Zaira and Port Zahir are across the water on the map; they are not silently included in this Alkebu study set.

## Landscape contracts

### ALK-01 — Red Sand Desert (`alkebu`)

**Source:** Red Sand Desert, lines 700–710. **Overview anchor:** [2700,1290].

**Canon:** once-fertile land transformed by Zephyra Scorchsong's genie pact during the War of Black Blood; magical red sands, forgotten temples/relics, traps and dangerous terrain.

**Implementation proposal:** rust/crimson/terracotta dunes, exposed dark rock and partly buried masonry. Exposed study has no ordinary vegetation or water. Dune forms and ruined architecture remain authored proposals, not a named temple plan. Avoid oasis palms, planted courts and prosperous buildings here. Do not reuse Sacred Fire temple insignia in an unknown ruin.

**Gameplay planning:** readable traversable dune saddles, buried thresholds and unstable-looking margins; actual traps or movement penalties need design and server rules. Terrain heights and collision must share one source when this becomes playable.

### ALK-02 — Menaka oasis gardens (`alkebu-oasis`)

**Source:** Menaka, 634–652; regional irrigation pact, 22–26. **Anchor:** [2590,1700].

**Canon:** lush oases and gardens, spiritual learning, pilgrimage, Great Temple of the Four Winds. Gardens are an inhabited microenvironment; they do not erase the surrounding landscape shown by the map.

**Proposal:** enclosed water court, managed channels, pale weathered stone, shade, concentrated planting and a small rest shelter. Palm species and layout are proposals. Do not copy Anathol's entire white-marble capital here or invent Four Winds iconography. The water intake is unresolved; the basin is not a claim of a mapped spring.

**Gameplay planning:** footpaths and crossings stay dry/readable; gathering only in designated plots, not every decorative leaf. Sanctuary/social use should reflect Menaka's role without assuming a universal combat ban.

### ALK-03 — Ataluk fertile plain (`alkebu-plain`)

**Source:** Ataluk, 497–515. **Anchor:** [2910,1522].

**Canon:** productive plain; fruit and vegetable cultivation, livestock, wool/silk textiles and a trading bazaar.

**Proposal:** rich soil in beds, orchard margins, channels and a sluice, field shelter and simple crossing. Crops are generic visual placeholders, not canon species or a production economy. Green follows cultivation and water. Avoid transforming farmland into wild jungle or putting continuous red dunes through it.

**Gameplay planning:** route through field margins; separate owned crops, harvestable resources, livestock and decoration. Require catchment/intake review before connecting channels to a named river.

### ALK-04 — Jungle of the Fangs (`alkebu-fangs`)

**Source:** Jungle of the Fangs, 774–784. **Anchor:** [2550,1525], map label Fang Forest.

**Canon:** Black Lion territory's tangled jungle, thorny vegetation, murky swamps, medicinal plants, hidden temples/ruins and dangerous predators; Tabaxi and Yuan-ti are mentioned in the site. The anchor is not a complete political boundary.

**Proposal:** layered broadleaf canopy, buttress roots, vines and understory surrounding broken dark pools. Narrow dry passage and a fallen trunk create useful silhouettes. Distinguish swamp water from clear mountain water. Avoid ornamental circular ponds, tidy plantations, sparse parkland, or alien luminous flora unsupported by lore. Specific medicinal plants and any inhabitants require their own designs; pots and broken walls do not establish a new settlement.

**Gameplay planning:** shared wet/dry mask, roots and occlusion; predators need readable approach space. Murky appearance is not automatic poison or impassability. Define actual hazards separately.

### ALK-05 — Dragon Fang ravine (`alkebu-dragon`)

**Source:** Dragon Fang Mountains, 738–746. **Study anchor:** [2960,1740], interpolated along the atlas ridge, not a named ravine pin.

**Canon:** high rugged southeastern mountains, waterfalls and clear rivers, nomadic communities and predators.

**Proposal:** heightfield ravine, ledged path, weathered rock faces, small cascade and sparse sheltered growth along the stream. No arctic snow blanket, volcanic glow or continuous red sand. The study is unnamed; no new canonical waterfall is created. Nomadic shelters are deferred until a camp's use and inhabitants are designed.

**Gameplay planning:** elevation and route continuity must be tested, not faked by camera angle. Treat waterfall, pool depth, ford/bridge and fall boundaries explicitly; connect drainage only after map reconciliation.

### ALK-06 — Flame Peaks approach (`alkebu-flame`)

**Source:** Sacred Fire temple, 760–772; Flame Peaks label/crater on map. **Study anchor:** [3180,1420].

**Canon:** rugged mountain sanctuary to Ethoras and Necis, red-stone temple with red/gold detail and two colossal stone warriors carrying spears/shields; sacred altar flame has a magical source.

**Proposal:** exposed rock, rubble and rising stair leading toward the sanctuary. This is a terrain/approach study below the temple; it does not substitute a lamp for the sacred altar or claim the omitted guardian sculptures are finished. Exact rock color and local votive light are proposals. No active lava field is inferred from the range name alone.

**Gameplay planning:** steep passage, sanctuary threshold and encounter clearance. The temple needs its own architecture study including the two guardians before full implementation.

### ALK-07 — Port Tanzane shore (`alkebu-coast`)

**Source:** Port Tanzane, 666–682. **Anchor:** [2498,1700], atlas key `port_tazane`.

**Canon:** coastal trading port with shipyards, repair shops, shipwrights and sailmakers. The map spelling is Port Tazane; public display follows the gazetteer.

**Proposal:** continuous shore/open water, salt-worn stone slipway, timber landing, mooring posts, repair shelter and exposed hull ribs. Hull is a repair asset, not a vessel implementation. Sparse coastal vegetation does not imply a resort beach. No specific tide, sand color, or sea name is canonized by the material choice.

**Gameplay planning:** pier heights, shore collision, embark points and water boundary must agree. Keep trade dressing distinct from loot. Do not relocate this study to Cerenan to sidestep its unresolved location.

## Other Alkebu places retained for later implementation

- **Anathol:** urban port/capital treatment, not a biome synonym. White marble, murals/mosaics, Great Citadel of Tarses, fortified port and markets need a dedicated city plan (301–323).
- **Dadu:** dry oasis-town construction explicitly includes stone and adobe, narrow streets and weekly markets (343–365). It should not inherit Anathol's monumental marble everywhere.
- **Kupa:** rocky hill fortress, stone buildings, red-tile roofs, narrow winding streets, military craft and brewing (597–615). This is the settlement treatment for appropriate terrain, not a new climate zone. Do not paint all Black Lion land dry merely because its capital is on a rocky hill; the Fang jungle is also explicit.
- **Cerenan:** coastal fishing/textile economy is in the gazetteer (559–581), but the atlas flags an inland/mountain placement. Keep the conflict visible until resolved.
- **Ivory Citadel:** white marble and crystalline towers belong to a specific Blue Moon site (712 onward). Those materials are not a universal Alkebu kit.

## Transitions and consistency during full implementation

These are rules for composing local terrain, not asserted direct adjacency between every pair of studies:

| Transition | Required continuity | Avoid |
|---|---|---|
| Dry ground → oasis/field | Traceable water, soil change, planting/cultivation edge | A global biome tint or instantly spawning palms |
| Dry margin → jungle | Increasing soil moisture and understory where geography supports it | Declaring an arbitrary direct Red Sands/Fang Forest boundary |
| Mountain → river corridor | Shared elevations, downslope drainage, sheltered vegetation | Flat water cutting through unrelated cliff heights |
| River/land → coast | Consistent shoreline, banks, pier and slipway heights | An isolated decorative pond standing in for the sea |
| Red Sands → other dry terrain | Preserve the magical scar's specific material identity | Making every sandy area red |
| Flame Peaks → Dragon Fangs | Separate range identities and catchments | Joining the two studies into one invented volcano |

All studies use the fixed isometric camera and existing material/leaf assets. Layouts are small review compositions, not compressed geographic maps. Final places need shared collision and ground heights, asset naming by region/site, resource placement rules, canopy/roof visibility, texture-density checks at gameplay zoom, and mobile performance measurements. The spike's visual checks verify rendering/layout, not lore correctness or playable navigation.

## Open geography and evidence issues

1. **Cerenan:** coastal prose versus inland atlas pin; do not silently choose a location.
2. **Peaks of Flame / Burning Blood Peaks:** atlas names remain separate; do not merge the ranges or their sacred sites without a decision.
3. **Anathol river:** `alkebu_anathol_river` points around x=2650–2755 do not meet Anathol's pin x=2980. The label alone is insufficient to wire hydrology. The Ataluk trace also needs endpoint review. Local channels in the studies are proposals, not validated river segments.
4. **Sea names and spellings:** Sand Sea/Alkebu Sea and map Port Tazane/prose Port Tanzane are recorded rather than rewritten. Coast study does not resolve naming.
5. **Political boundaries:** neither study pins nor forest icons define full clan territories.
6. **Night Wind:** the desert passage calls the clan extinct then mentions practitioners. No definitive living heraldry is invented.

For the next production pass, choose a named locality, use the shared record above, then resolve only the map issues that affect that locality. Do not move to the next world region until Alkebu's reviewed treatments and their limitations are carried forward.
