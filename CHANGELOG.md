# Changelog

## v0.5 - Locality pass - 2026-10-2
- Expanded from 125 to 166 specimen records.
- Expanded from 88 to 90 taxon records.
- Added new `locality_audit.csv` to track, locality by locality, how complete each search actually is instead of just accumulating records.
- The new `Locality_audit` currently shows:
- Pant-y-ffynnon: 39 registered records
- Pontnewydd: 24
- Coygan: 13
- Pant Quarry 2: 8
- Paviland: 6
- Pontalun 3: 4
- Pontalun 2: 3
- Improved Pant-y-ffynnon, The database now separates the multi-part Terrestrisuchus gracilis holotype into its actual catalogue components—PV R 7557a, b, c, existing d, then e–h—and adds the principal associated specimens such as PV R 7553a–b, 7561a–c, 7562, 7571, 7591, 7593a–e, 37600a–e, 37788, and 37726.
- Expanded Clevosaurus cambrica properly.

## v0.4 - Third pass - 2026-09-19
- The Specimens structured table now actually extends through all 125 rows, so filters/sorting include the new material.
- The search audit has been updated to show Museum Wales, NHMUK and GB3D as still “In progress”, rather than falsely implying those catalogues have been exhausted.
- Ambiguous labels such as “Merck's rhinoceros” remain source-faithful instead of receiving a guessed modern species.
- PV M 26368, currently identified online as Eozostrodon parvus but with a historical Morganucodon determination, has its taxonomic history flagged for investigation rather than silently overwritten.
- Sensitive cave and fissure localities continue to be marked Restricted.
- Digital imagery/CT/GB3D resources are linked through the Digital_assets table.
- Expanded from 79 to 125 specimen records.
- Expanded from 59 to 88 taxon records.
- Expanded locality coverage to 54 records.

## v0.3 — Second pass — 2026-09-12

- Expanded from 36 to 79 specimen records.
- Expanded from 27 to 59 taxon records.
- Expanded locality coverage to 44 records.
- Added further geological-unit normalisation.
- Added Sedgwick Museum, British Geological Survey, and Grosvenor Museum as repositories.
- Added GB3D Type Fossils Online as a major cross-institution discovery source.
- Added 27 digital-asset records, principally linked to GB3D imagery and NHMUK IIIF resources.
- Added additional Museum Wales holotypes and paratypes.
- Added additional NHMUK Pant/Pontalun fissure material and other Welsh records.
- Improved provenance for selected Museum Wales type specimens using GB3D.
- Added unresolved questions for conflicting type status, nomenclature, and stratigraphy.

## v0.2 — First pass — 2026-09-12

- Populated the first specimen-level working dataset.
- Added Museum Wales type records.
- Added selected NHMUK records from Pant-y-ffynnon, Pant Quarry, Llanover, and other localities.
- Added major Welsh vertebrate records including *Dracoraptor*, *Pendraig*, *Aenigmaspina*, *Gephyrosaurus*, and *Morganucodon*.
- Added initial locality and geological-unit tables.
- Added unresolved-question workflow.

## v0.1 — Schema release

- Established relational workbook structure.
- Added search queue, candidate staging tables, repository watchlist, dashboard, and research protocol.
